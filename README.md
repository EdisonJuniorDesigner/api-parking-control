
# API Spot Parking

Uma API de estacionamento para condomínios.

Tendo a inserção dos automóveis nas vagas do devidos condôminos, assim como listagem, alteração e deleção dos dados.

<hr>

## Stack utilizada

**Back-end:** Spring Boot, Spring JPA, Validation, PostgreSQL Driver

**Banco de dados:** PostgreSQL

**Ferramentas:** pgAdmin4, SpringToolSuite4, Postman, Git

**Sistema Operacional:** Linux Ubuntu 22.04

<table>
  <tr>
    <td>
      <img src="https://badgen.net/npm/license/lodash">
    </td>
    <td>
      <img src="https://badgen.net/maven/v/metadata-url/https/repo1.maven.org/maven2/com/google/code/gson/gson/maven-metadata.xml">
    </td>
    <td>
      <img src="https://badgen.net/badge/icon/git?icon=git&label">
    </td>
    <td>
      <img src="https://badgen.net/badge/icon/github?icon=github&label">
    </td>
  </tr>
</table>

<hr>


## Documentação da API

#### Retorna todos os itens (Paginação default, size = 10)

```http
  GET /api/parking-spot
```

| Parâmetro   | Tipo       | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `api_key` | `string` | **Obrigatório**. A chave da sua API |

#### Retorna todos os itens por página

```http
  GET /api/parking-spot?page=0&size=5&sort=registrationDate,ASC
```

| Parâmetro   | Tipo       | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `api_key` | `string` | **Obrigatório**. A chave da sua API |

#### Retorna um item

```http
  GET /api/parking-spot/${id}
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `id`      | `string` | **Obrigatório**. O ID do item que você quer listar |

#### Deleta um item

```http
  DELETE /api/parking-spot/${id}
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `id`      | `string` | **Obrigatório**. O ID do item que você quer deletar|

#### Atualiza um item

```http
  PUT /api/parking-spot/${id}
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `id`      | `string` | **Obrigatório**. O ID do item que você quer atualizar|

<hr>

## Autor

- [@EdisonJuniorDesigner](https://github.com/EdisonJuniorDesigner)
<table>
 <tr>
    <td>
      <img src="https://avatars.githubusercontent.com/u/44264221?v=4" width="130px">
      <p>Edison Junior</p>
    </td>
  </tr>
</table>

