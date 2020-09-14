# Teste Genoa - Backend

## Requisitos obrigatórios

- Node.js
- MySQL

## Instruções

- Você deve criar um CRUD(POST, GET, PUT, DELETE)
- Você é livre para utilizar as libs que quiser
- O case é baseado em uma contratação ficticia, a tabela deve ser baseada nessa:

id | cnpj            | razao_social  | data_inicio | data_final | ativo_total | abertura_empresa
-- | --------------- | ------------  | ----------- | ---------- | ----------- | --------------
1  | 12345678901122  | nomedaempresa | 11/09/2020  | 11/09/2021 | R$1500000   | 10/03/2002

* CRUD - permitir inserir nova empresa, listar dados do banco, atualizar dados da empresa e deletar empresa
* data_inicio/data_final - duração do seguro
* abertura_empresa - data de fundação da empresa

# Regras de negócio
1. validações de campos em branco
2. CNPJ pode ser incluido como XX.XXX.XXX/0001-XX, então a validação deve retirar caracteres especiais
3. data_inicio não pode ser maior que data_final
4. data_final deve ser 1 ano após a data_inicio
5. se o ativo total for menor que R$1000000 e maior que R$153000000, deverá retornar uma mensagem negando a contratação
6. se a empresa estiver aberta a menos de 2 anos(abertura_empresa) deverá retornar uma mensagem negando a contratação

## Duvidas ou entrega

* Dúvidas e entregas devem ser enviadas para rodrigo.pedroni@genoaseguros.com.br ou rodrigo.tanaka@genoaseguros.com.br
* Mandar o link do repositorio ou .zip sem a pasta node_modules
