# Response Models

Todo EndPoint da API produz uma resposta no formato já explicado [aqui](request-response.html) e para facilitar a compreensão dos dados, essa seção visa explicar os **Models** que podem vir no Payload e seus atributos.

Na API os models apenas vem explícitos quando estão sendo referenciados junto à outros models. Como por exemplo, o EndPoint **getDevice** possui o model **resources** que é uma lista de models **resource**.

## O que é um Model

Um modelo de dados ( Model ) é uma abstração de dados que representa algum dado no mundo real. Isto é, uma representação dos dados no nosso sistema de forma clara e objetiva.

Models
-----------------

## Resource Model

```
{
            "id_resource": 19,
            "id_device": 8,
            "id_resource_subtype": 3,
            "id_last_feed": 186864,
            "name": "Rele",
            "description": "",
            "lifetime": 1,
            "lifetime_updated_at": "2017-08-07 19:50:47",
            "created_at": "2017-05-22 20:12:24",
            "updated_at": "2017-08-02 23:52:00",
            "active": 1,
            "is_alive": false,
            "subtype": {
                "id_resource_subtype": 3,
                "id_resource_type": 1,
                "name": "Binário",
                "name_i18n": "Binary",
                "description": null,
                "data_format_operation": 0,
                "data_restriction_regex": null,
                "data_restriction_begin_range": 0,
                "data_restriction_end_range": 1,
                "created_at": "2017-05-10 00:00:00",
                "updated_at": "2017-05-10 00:00:00"
            },
            "last_feed": {
                "id_resource_feed": 186864,
                "id_resource": 19,
                "raw_data": "0",
                "created_at": "2017-08-02 23:52:00"
            },
            "data_format": [
                {
                    "id_resource_data_format": 26,
                    "id_resource": 19,
                    "id_logical_operator": null,
                    "name": "Desligado",
                    "value": "0",
                    "created_at": "2017-05-26 22:37:46",
                    "updated_at": "2017-06-01 22:31:19",
                    "active": 1
                },
                {
                    "id_resource_data_format": 27,
                    "id_resource": 19,
                    "id_logical_operator": null,
                    "name": "Ligado",
                    "value": "1",
                    "created_at": "2017-05-26 22:37:46",
                    "updated_at": "2017-06-01 22:31:27",
                    "active": 1
                }
            ]
        }
```
