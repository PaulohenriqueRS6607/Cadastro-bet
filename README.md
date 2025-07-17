# Bet - Cadastro de Usuários

Este projeto é um cadastro simples de usuários, desenvolvido durante uma aula prática, utilizando como base o conceito de uma plataforma de apostas (bet).

## Requisitos

- **Java 21**
- **Maven**
- **MySQL** (ou outro banco compatível, ajustar em `application.properties`)

## Configuração

1. Clone o repositório.
2. Configure o banco de dados MySQL conforme o arquivo `src/main/resources/application.properties`:
   ```
   spring.datasource.url=jdbc:mysql://localhost:3306/crud
   spring.datasource.username=root
   spring.datasource.password=
   ```
## Endpoints

Todos os endpoints estão sob o path `/api`:

| Método  | URL                | Descrição                |
|---------|--------------------|--------------------------|
| POST    | `/api/cadastrar`   | Cadastra um novo usuário |

## Exemplo de JSON para cadastro

```json
{
  "cpf": "12345678900",
  "senha": "minhaSenhaSegura",
  "aniver": "2000-01-01",
  "email": "usuario@email.com"
}
```

## Observações

- O projeto utiliza Spring Data JPA e Lombok.
- O banco de dados é atualizado automaticamente (`spring.jpa.hibernate.ddl-auto=update`).
- O login e senha do banco devem ser ajustados conforme seu ambiente.
- Este projeto tem fins exclusivamente educacionais, servindo como exemplo para aulas e estudos sobre desenvolvimento backend e estruturação de projetos Java. 
