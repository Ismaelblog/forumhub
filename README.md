<p align="center">
  <img src="https://www.esperantina.to.gov.br/storage/noticias/1428522025020567a39fd473910.png" alt="Print do Menu" width="500">
</p>

# 🏁 ForumHub - Challenge Alura

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)

O **ForumHub** é uma API REST desenvolvida como desafio final do programa Oracle Next Education (ONE) em parceria com a Alura. O objetivo é replicar o comportamento de um fórum, onde usuários podem se autenticar e gerenciar tópicos de discussão.

---

## 🛠️ Funcionalidades

- **Autenticação Segura:** Sistema de login utilizando Spring Security e BCrypt para criptografia de senhas.
- **Tokens JWT:** Geração e validação de tokens para acesso às rotas protegidas.
- **CRUD de Tópicos:** Criação, listagem (com paginação), detalhamento, atualização e exclusão de tópicos.
- **Validação de Dados:** Uso de Bean Validation para garantir a integridade das informações.
- **Tratamento de Erros:** Respostas JSON customizadas para erros de validação e recursos não encontrados.

---

## 🚀 Tecnologias Utilizadas

- **Java 21**
- **Spring Boot 3**
- **Spring Data JPA** (Persistência de dados)
- **Spring Security** (Segurança e Autenticação)
- **Auth0 JWT** (Tokens de acesso)
- **MySQL** (Banco de dados relacional)
- **Maven** (Gerenciador de dependências)

---

## 📋 Como Executar o Projeto

1. Clone o repositório:
   `git clone https://github.com/SEU_USUARIO/forumhub.git`

2. Configure o banco de dados no arquivo `src/main/resources/application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/forumhub_api
   spring.datasource.username=seu_usuario
   spring.datasource.password=sua_senha

3. Execute a aplicação via IntelliJ ou terminal:
```mvn spring-boot:run```
---

## 🔌 Endpoints Principais

| Método | Endpoint | Descrição | Acesso |
| --- | --- | --- | ---|
| POST | /login | Autentica usuário e gera Token | Público |
| GET | /topicos | Lista todos os tópicos (paginado) | Privado |
| POST | /topicos | Cadastra um novo tópico | Privado |
| GET | /topicos/{id} | Detalha um tópico específico | Privado |
| PUT | /topicos/{id} | Atualiza dados de um tópico | Privado |
| DELETE | /topicos/{id} | Remove um tópico | Privado |

---
<div align="center">

### Desenvolvido por Ismael Fernandes 👋

</div>
