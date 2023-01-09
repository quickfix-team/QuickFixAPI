# QuickFixAPI

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

GET  /profiles/id <br/>
POST /profiles/id <br/>
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

POST /adresses/id <br/>
PUT  /adresses/id <br/>
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

POST /contacts/id <br/>
PUT  /contacts/id <br/>
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
