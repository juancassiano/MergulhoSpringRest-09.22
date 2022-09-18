
# Algalog
![](msr.png)

Projeto desenvolvido durante o Mergulho Spring Rest - Setembro de 2022 - Pela Algaworks

![Diagrama](diagrama.png)

## Rotas da API

#### Cadastra cliente
```http
 POST /clientes
```
Corpo em JSON
```
{
    "nome": "Maria",
    "email": "maria@email.com",
    "telefone": "21 99999 9999"
},
```

### Retorna o cliente especificado no parâmetro
```http
 GET /clientes/{id}
```

 #### Retorna todos os clientes registrados
```http
 GET /clientes
```
#### Atualiza os dados do cliente especificado no parâmetro
```http
 PUT /clientes/{id}
 ```
#### Exclui o clientes especificado no parâmetro
```http
 DELETE /clientes/{id}
```

#### Retorna todas as entregas registrados
```http
 GET /entregas
```

#### Cadastra entrega
```http
 POST /entregas
```
Corpo em JSON
```
{
    "cliente":{
        "id": "2"
    },
    "destinatario":{
        "nome": "Joaquim da Silva",
        "logradouro": "Rua das Goiabas",
        "numero": "100",
        "bairro": "Centro",
        "complemento":"fundos"
    },
    "taxa":100.50
}
```

#### Retorna dados de determinada entrega registrados
```http
 GET /entregas/{id}
```
#### Finaliza entrega passada no parâmetro
```http
 PUT /entregas/{id}/finalizacao
```

#### Cadastra ocorrênia para determinada entrega registrada no parâmetro
```http
 GET /entregas/{id}/ocorrencias
```
Corpo em JSON
```
{
    "descricao": "Tentativa sem sucesso"
},
```


#### Retorna as ocorrências de determinada entrega passada no parâmetro
```http
 GET /entregas/{id}/ocorrencias
```


## Tecnologias
[Spring Boot](https://spring.io/projects/spring-boot)

[Java JPA](https://jakarta.ee/specifications/persistence/)

[MySQL](https://dev.mysql.com/doc/)

[Flyway](https://flywaydb.org/documentation/)

[Lombok](https://projectlombok.org/)

[ModelMapper](http://modelmapper.org/getting-started/)

[Postman](https://www.postman.com/)
## Ferramentas

<div style="display: inline_block"><br>

<img align="center" height="50" width="150" src="https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white"/>
<img align="center" height="50" width="150" src="https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white"/>
<img align="center" height="50" width="150" src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white"/>

</div>