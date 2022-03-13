# json-server-base

Esse é o repositório com a base de JSON-Server + JSON-Server-Auth já configurada, feita para ser usada no desenvolvimento das API's nos Capstones do Q2.

## Endpoints

Assim como a documentação do JSON-Server-Auth traz (https://www.npmjs.com/package/json-server-auth), existem 3 endpoints que podem ser utilizados para cadastro e 2 endpoints que podem ser usados para login.

### Cadastro

POST /register <br/>
POST /signup <br/>
POST /users

Qualquer um desses 3 endpoints irá cadastrar o usuário na lista de "Users", sendo que os campos obrigatórios são os de email e password.
Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.


### Login

POST /login <br/>
POST /signin

Qualquer um desses 2 endpoints pode ser usado para realizar login com um dos usuários cadastrados na lista de "Users".

### Cart

POST/cart

Neste endepoint somente o usuario autenticado pode adicionar um novo item no carrinho, ele tambem precisa na requicao , a referencia do id do usuario ex:"userID:1".

GET/cart

Neste endpoint qualquer pessoa pode acessar , sem a necessidade de autenticação.

### infoUser

POST/infoUser
GET/infoUser

Nestes 2 endpoint somente o usuario autenticado pode Registrar e acessar estas informações .

POST/  ele  precisa na requicao a referencia do id do usuario ex:"userID:1".

