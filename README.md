
## Back-end com NodeJS

### 📖 Sobre:
O projeto trata-se de um back-end simples que recebe requisições HTTP através do http://localhost:3333/ e salva os dados em um array do próprio código.

Nesse projeto também foi desenvolvido uma Middleware para validar o ID do projeto como UUID quando é feito alguma solicitação com parametro de ID.


### 🔧 Para rodar esse projeto:

1- Instale as libs com o comando **yarn**.
2- Rode o projeto com o comando **yarn dev***.


### 📍 As requisições aceitas são:

+ **GET** (/projects) para **listar** todos os projetos salvos.

+ A resposta é dada em uma lista de projetos. Como abaixo:
```JSON
[
  {
    "id": "cc50e992-37bd-417c-8c70-15dc6c670308",
    "title": "Projeto 1",
    "owner": "Gabriela1"
  },
  {
    "id": "67a55f53-ac3d-4eb4-acf7-4dba29c24b07",
    "title": "Projeto 2",
    "owner": "Gabriela2"
  },
  {
    "id": "ed040e28-b4b7-42b2-889e-3f69afee8902",
    "title": "Projeto 3",
    "owner": "Gabriela3"
  }
]
```

+ **POST** (/projects) para **criar** um novo projeto.

  + Deve-se enviar os dados no corpo da requisição. Como abaixo:

```JSON
{
	"title": "Projeto 1",
	"owner": "Gabriela"
}
```

+ **PUT** (/projects/valor_do_id) para **editar** um projeto existente.

  + Deve-se enviar os dados a serem editador no corpo da requisição. Como abaixo:

```JSON
{
	"title": "Projeto 1",
	"owner": "Gabriela"
}
```

+ **DELETE** (/projects/valor_do_id) para **deletar** um projeto existente.

  + Nessa requisição não há nada no corpo, apenas o ID como parametro na URL.


##
Desenvolvido por Gabriela Queiroz ! 💜
