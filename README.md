
# API Spot Parking

Uma API de estacionamento para condomínios.

Tendo a inserção dos automóveis nas vagas do devidos condôminos, assim como listagem, alteração e deleção dos dados.



## Stack utilizada

**Back-end:** Spring Boot, Spring JPA, Validation

**Banco de dados:** PostgreSQL




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


## Autor

- [@EdisonJuniorDesigner](https://github.com/EdisonJuniorDesigner)

