# AV2 - Spring Boot API com JWT, Segurança e Monitoramento

## Descrição
API RESTful construída com Spring Boot 3.x que implementa autenticação JWT, autorização, monitoramento com Actuator, Prometheus e Grafana, além de testes unitários e containerização com Docker.
---

## Requisitos
- Java 17+
- Maven 3.8+
- Docker (opcional, para deploy via container)
- Git (para versionamento)
- Conta no Railway (para deploy gratuito)
---

## Instalação
1. Clone o repositório
2. Buildar o projeto com Maven
3. Execute o JAR gerado:
java -jar target/demo-0.0.1-SNAPSHOT.jar

A API estará disponível em:
http://localhost:8080
---

## Testes
Execute os testes unitários com:
mvn test
---

## Monitoramento
Endpoints de monitoramento disponíveis via Actuator:
Saúde: http://localhost:8080/actuator/health
Métricas: http://localhost:8080/actuator/metrics
Prometheus: http://localhost:8080/actuator/prometheus
---

## Docker
Buildar a imagem Docker:
docker build -t av2dianaalves .

Rodar a aplicação em container:
docker run -p 8080:8080 av2dianaalves
---

## Swagger / OpenAPI
Acesse a documentação interativa via Swagger UI em:
http://localhost:8080/swagger-ui.html