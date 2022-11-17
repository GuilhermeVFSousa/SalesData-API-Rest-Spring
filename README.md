
## Sales Data API Rest

Endpoint: https://dsmeta-gvfs.herokuapp.com/sales

Endpoint com parâmetros: https://dsmeta-gvfs.herokuapp.com/sales?minDate=2021-11-01&maxDate=2021-12-31



O projeto consitem em:
- API Rest com Java e Spring Boot
- Banco de Dados em memória (H2)
- Integração com notificação via SMS
- Implantação em nuvem com integração contínua(CI) e entrega contínua(CD), utilizando o Heroku


### Banco de dados
- Criação das entidades
- Mapeamento objeto-relacional (JPA)
- Configuração de dados de conexão do banco de dados H2
- Seed do banco de dados

### Endpoint da API REST
- Repository
- Service
- Controller

### Envio de notificação via SMS utilizando a plataforma Twilio
Dependências Maven do Twilio
```java
  <dependency>
	<groupId>com.twilio.sdk</groupId>
	<artifactId>twilio</artifactId>
	<version>8.31.1</version>
</dependency>
```
### Variáveis de ambiente necessárias

```java
twilio.sid=${TWILIO_SID}
twilio.key=${TWILIO_KEY}
twilio.phone.from=${TWILIO_PHONE_FROM}
twilio.phone.to=${TWILIO_PHONE_TO}
```
### Implantação no Heroku
```java
Arquivo system.properties

java.runtime.version=17
```



