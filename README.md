# CRUD de Produtos - API

API REST em Spring Boot com persistencia em PostgreSQL (JPA).
Atividades 18-20 - Sistemas Distribuidos e Mobile (Anhembi Morumbi, 2026/2).

## Endpoints
| Metodo | Rota | Resposta |
|---|---|---|
| GET | /produtos | 200 - lista |
| GET | /produtos/{id} | 200 ou 404 |
| POST | /produtos | 201 |
| PUT | /produtos/{id} | 200 ou 404 |
| DELETE | /produtos/{id} | 204 ou 404 |

## Variaveis de ambiente
| Variavel | Padrao | Uso |
|---|---|---|
| PORT | 8081 | Porta HTTP |
| SPRING_DATASOURCE_URL | H2 em memoria | ex.: jdbc:postgresql://host:5432/banco |
| SPRING_DATASOURCE_USERNAME / _PASSWORD | sa / vazio | Credenciais do banco |
| CORS_ORIGINS | * | Origens do front liberadas |

## Rodar
```
./mvnw spring-boot:run
```
Deploy no Render: Web Service com runtime Docker (Dockerfile na raiz).