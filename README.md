# Teste Genoa - Backend

## Requisitos obrigatórios

- Node.js
- MySQL

## Instruções

- Você deve criar uma API REST e incluir um CRUD(GET, POST, PUT, DELETE)
- Você é livre para utilizar as libs que quiser
- O case é baseado em uma contratação ficticia, a tabela deve ser baseada nessa:

id | cnpj            | razao_social  | data_inicio | data_final | ativo_total 
-- | --------------- | ------------  | ----------- | ---------- | -----------
1  | 12345678901122  | nomedaempresa | 11/09/2020  | 11/09/2021 | R$1500000
2  | 12345678901122  | nomedaempresa | 11/09/2020  | 11/09/2021 | R$1500000

* validações de campos em branco
* CNPJ pode ser incluido como XX.XXX.XXX/0001-XX, então a validação deve retirar caracteres especiais
* data_inicio não pode ser maior que data_final
* data_final deve ser pelo menos 1 ano a mais que a data_inicio
* se o ativo total for menor que R$1000000 e maior que R$153000000, deverá recursar a requisição

## Duvidas ou entrega

* Dúvidas e entregas devem ser enviadas para rodrigo.pedroni@genoaseguros.com.br ou rodrigo.tanaka@genoaseguros.com.br
* Mandar o link do repositorio ou .zip sem a pasta node_modules
