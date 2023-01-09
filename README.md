# json-server-base

Esse é o repositório com a base de JSON-Server + JSON-Server-Auth já configurada, feita para ser usada no desenvolvimento das API's nos Projetos Front-end.

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

Qualquer um desses 2 endpoints pode ser usado para realizar login com um dos usuários cadastrados na lista de "Users"

### Profile 

GET  /profiles/id
POST /profiles/id
PUT  /profiles/id

Retorno
```
  {
	"profileId": 1,
	"street": "Gen. Mário Tourinho",
	"district": "Seminário",
	"number": "1733",
	"city": "Gramados",
	"state": "PR",
	"id": 1
}
```

### Adresses 

POST /adresses/id
PUT  /adresses/id
GET  /adresses/id

```
{
	"profileId": 1,
	"street": "Gen. Mário Tourinho",
	"district": "Seminário",
	"number": "1733",
	"city": "Curitiba",
	"state": "PR",
	"id": 1
}
```

### Contacts

POST /contacts/id
PUT  /contacts/id
GET  /adresses/id

```
{
	"id": 1,
	"profileId": 1,
	"phone": "(41) 99108-7575",
	"whatsapp": "(41) 99108-7575",
	"instagram": "kenzieacademybr",
	"email": "kenzinho@mail.com",
	"telegram": "(41) 99108-7575"
}
```
