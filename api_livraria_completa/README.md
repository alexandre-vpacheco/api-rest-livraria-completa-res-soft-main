# Descrição
API Rest utilizando Spring Boot.

## Dependências e Versões

* Java - v 17
* Spring Boot - v 3.0.6
* Spring Security
* H2 Database
* Swagger (com springdoc)
* Jsonwebtoken

## Endpoints Principais - Autenticação

```bash
/roles (criação de roles)
/auth/signup (criação de usuários)
/auth/signin (login de usuários)
```

## Endpoints Principais - Negócios

```bash
/autores 
/editoras
/livros
/livros/por-editora/{id}
```

### Endpoints com Paginação

* Os parâmetros pagina e qtdRegistros são números inteiros
* Os parâmetros acima são opcionais
* A paginação se inícia na página 0
* Os valores dos parâmetros deverão ser modificados de acordo com os registros que se deseja obter

```bash
/editoras?pagina=0&qtdRegistros=2
/livros?pagina=0&qtdRegistros=2
/livros/por-editora/{id}?pagina=0&qtdRegistros=2
```

## Endpoints - Coleção de todos os Endpoints para Insomnia

```bash
Insomnia_Endpoints_Collection.json
```

## Executando

```bash
mvnw spring-boot:run
```
## Licença

GNU GPL

```properties
spring_profiles_active=prod
PROD_DB_HOST=containers-us-west-23.railway.app
PROD_DB_PORT=5844
PROD_DB_NAME=railway
PROD_DB_PASSWORD=L3QuISzR0iBeivz4qxdN
PROD_DB_USERNAME=postgres
```
