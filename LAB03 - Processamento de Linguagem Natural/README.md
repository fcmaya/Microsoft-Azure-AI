
# Análise de Sentimentos com o Language Studio no Azure AI


## Azure AI Speech

O serviço de Fala de IA do Azure transcreve fala em texto e texto em fala audível. Pode-se usar o AI Speech para criar um aplicativo que possa transcrever anotações de reuniões ou gerar texto a partir da gravação de entrevistas.

Neste exercício, utilizamos os recursos do Azure AI Speech usando o Azure AI Speech Studio.

### Execução

Foi selecionado o serviço "Real-time speech to text" (Conversão de voz em texto em tempo real).

Após importar o arquivo de audio WhatAICanDo.m4a e executar o teste, o texto narrado é exibido abaixo e o seu JSON correspondente.

"AI enables us to build amazing software that can improve healthcare, enable people to overcome physical disadvantages. Empower smart infrastructure, create incredible entertainment experiences, and even save the planet. "

"A IA nos permite construir softwares incríveis que podem melhorar os cuidados de saúde, permitir que as pessoas superem desvantagens físicas. Capacite a infraestrutura inteligente, crie experiências de entretenimento incríveis e até salve o planeta. "

<details>
  <summary>Clique para exibir/ocultar o JSON</summary>
  
```json
[
    {
        "Id": "7590ca40774a41249274f005b89f1d2c",
        "RecognitionStatus": 0,
        "Offset": 12800000,
        "Duration": 72400000,
        "Channel": 0,
        "DisplayText": "AI enables us to build amazing software that can improve healthcare, enable people to overcome physical disadvantages.",
        "NBest": [
            {
                "Confidence": 0.8962598,
                "Lexical": "AI enables us to build amazing software that can improve healthcare enable people to overcome physical disadvantages",
                "ITN": "AI enables us to build amazing software that can improve healthcare enable people to overcome physical disadvantages",
                "MaskedITN": "ai enables us to build amazing software that can improve healthcare enable people to overcome physical disadvantages",
                "Display": "AI enables us to build amazing software that can improve healthcare, enable people to overcome physical disadvantages.",
                "Words": [
                    {
                        "Word": "AI",
                        "Offset": 12800000,
                        "Duration": 800000
                    },
                    {
                        "Word": "enables",
                        "Offset": 13600000,
                        "Duration": 6800000
                    },
                    {
                        "Word": "us",
                        "Offset": 20400000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "to",
                        "Offset": 21600000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "build",
                        "Offset": 22800000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "amazing",
                        "Offset": 26000000,
                        "Duration": 6000000
                    },
                    {
                        "Word": "software",
                        "Offset": 32000000,
                        "Duration": 6400000
                    },
                    {
                        "Word": "that",
                        "Offset": 38400000,
                        "Duration": 1600000
                    },
                    {
                        "Word": "can",
                        "Offset": 40000000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "improve",
                        "Offset": 41200000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "healthcare",
                        "Offset": 44400000,
                        "Duration": 8000000
                    },
                    {
                        "Word": "enable",
                        "Offset": 55600000,
                        "Duration": 4000000
                    },
                    {
                        "Word": "people",
                        "Offset": 59600000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "to",
                        "Offset": 62800000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "overcome",
                        "Offset": 64000000,
                        "Duration": 4800000
                    },
                    {
                        "Word": "physical",
                        "Offset": 68800000,
                        "Duration": 4000000
                    },
                    {
                        "Word": "disadvantages",
                        "Offset": 72800000,
                        "Duration": 12400000
                    }
                ]
            },
            {
                "Confidence": 0.8668942,
                "Lexical": "ai enables us to build amazing software that can improve health care enable people to overcome physical disadvantages",
                "ITN": "ai enables us to build amazing software that can improve health care enable people to overcome physical disadvantages",
                "MaskedITN": "ai enables us to build amazing software that can improve health care enable people to overcome physical disadvantages",
                "Display": "AI enables us to build amazing software that can improve health care enable people to overcome physical disadvantages",
                "Words": [
                    {
                        "Word": "AI",
                        "Offset": 12800000,
                        "Duration": 800000
                    },
                    {
                        "Word": "enables",
                        "Offset": 13600000,
                        "Duration": 6800000
                    },
                    {
                        "Word": "us",
                        "Offset": 20400000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "to",
                        "Offset": 21600000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "build",
                        "Offset": 22800000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "amazing",
                        "Offset": 26000000,
                        "Duration": 6000000
                    },
                    {
                        "Word": "software",
                        "Offset": 32000000,
                        "Duration": 6400000
                    },
                    {
                        "Word": "that",
                        "Offset": 38400000,
                        "Duration": 1600000
                    },
                    {
                        "Word": "can",
                        "Offset": 40000000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "improve",
                        "Offset": 41200000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "health",
                        "Offset": 44400000,
                        "Duration": 2800000
                    },
                    {
                        "Word": "care",
                        "Offset": 47200000,
                        "Duration": 5200000
                    },
                    {
                        "Word": "enable",
                        "Offset": 55600000,
                        "Duration": 4000000
                    },
                    {
                        "Word": "people",
                        "Offset": 59600000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "to",
                        "Offset": 62800000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "overcome",
                        "Offset": 64000000,
                        "Duration": 4800000
                    },
                    {
                        "Word": "physical",
                        "Offset": 68800000,
                        "Duration": 4000000
                    },
                    {
                        "Word": "disadvantages",
                        "Offset": 72800000,
                        "Duration": 8400000
                    }
                ]
            },
            {
                "Confidence": 0.84675646,
                "Lexical": "ai enables us to build amazing software that can improve healthcare enable people to overcome physical disadvantages empower",
                "ITN": "ai enables us to build amazing software that can improve healthcare enable people to overcome physical disadvantages empower",
                "MaskedITN": "ai enables us to build amazing software that can improve healthcare enable people to overcome physical disadvantages empower",
                "Display": "AI enables us to build amazing software that can improve healthcare enable people to overcome physical disadvantages empower",
                "Words": [
                    {
                        "Word": "AI",
                        "Offset": 12800000,
                        "Duration": 800000
                    },
                    {
                        "Word": "enables",
                        "Offset": 13600000,
                        "Duration": 6800000
                    },
                    {
                        "Word": "us",
                        "Offset": 20400000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "to",
                        "Offset": 21600000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "build",
                        "Offset": 22800000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "amazing",
                        "Offset": 26000000,
                        "Duration": 6000000
                    },
                    {
                        "Word": "software",
                        "Offset": 32000000,
                        "Duration": 6400000
                    },
                    {
                        "Word": "that",
                        "Offset": 38400000,
                        "Duration": 1600000
                    },
                    {
                        "Word": "can",
                        "Offset": 40000000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "improve",
                        "Offset": 41200000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "healthcare",
                        "Offset": 44400000,
                        "Duration": 8000000
                    },
                    {
                        "Word": "enable",
                        "Offset": 55600000,
                        "Duration": 4000000
                    },
                    {
                        "Word": "people",
                        "Offset": 59600000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "to",
                        "Offset": 62800000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "overcome",
                        "Offset": 64000000,
                        "Duration": 4800000
                    },
                    {
                        "Word": "physical",
                        "Offset": 68800000,
                        "Duration": 4000000
                    },
                    {
                        "Word": "disadvantages",
                        "Offset": 72800000,
                        "Duration": 12400000
                    },
                    {
                        "Word": "empower",
                        "Offset": 89200000,
                        "Duration": 6400000
                    }
                ]
            },
            {
                "Confidence": 0.82154197,
                "Lexical": "ai enables us to build amazing software that can improve health care enable people to overcome physical disadvantages empower",
                "ITN": "ai enables us to build amazing software that can improve health care enable people to overcome physical disadvantages empower",
                "MaskedITN": "ai enables us to build amazing software that can improve health care enable people to overcome physical disadvantages empower",
                "Display": "AI enables us to build amazing software that can improve health care enable people to overcome physical disadvantages empower",
                "Words": [
                    {
                        "Word": "AI",
                        "Offset": 12800000,
                        "Duration": 800000
                    },
                    {
                        "Word": "enables",
                        "Offset": 13600000,
                        "Duration": 6800000
                    },
                    {
                        "Word": "us",
                        "Offset": 20400000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "to",
                        "Offset": 21600000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "build",
                        "Offset": 22800000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "amazing",
                        "Offset": 26000000,
                        "Duration": 6000000
                    },
                    {
                        "Word": "software",
                        "Offset": 32000000,
                        "Duration": 6400000
                    },
                    {
                        "Word": "that",
                        "Offset": 38400000,
                        "Duration": 1600000
                    },
                    {
                        "Word": "can",
                        "Offset": 40000000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "improve",
                        "Offset": 41200000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "health",
                        "Offset": 44400000,
                        "Duration": 2800000
                    },
                    {
                        "Word": "care",
                        "Offset": 47200000,
                        "Duration": 5200000
                    },
                    {
                        "Word": "enable",
                        "Offset": 55600000,
                        "Duration": 4000000
                    },
                    {
                        "Word": "people",
                        "Offset": 59600000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "to",
                        "Offset": 62800000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "overcome",
                        "Offset": 64000000,
                        "Duration": 4800000
                    },
                    {
                        "Word": "physical",
                        "Offset": 68800000,
                        "Duration": 4000000
                    },
                    {
                        "Word": "disadvantages",
                        "Offset": 72800000,
                        "Duration": 12400000
                    },
                    {
                        "Word": "empower",
                        "Offset": 89200000,
                        "Duration": 6400000
                    }
                ]
            },
            {
                "Confidence": 0.78071815,
                "Lexical": "ai enables us to build amazing software that can improve health care enable people to overcome physical disadvantages and power",
                "ITN": "ai enables us to build amazing software that can improve health care enable people to overcome physical disadvantages and power",
                "MaskedITN": "ai enables us to build amazing software that can improve health care enable people to overcome physical disadvantages and power",
                "Display": "AI enables us to build amazing software that can improve health care enable people to overcome physical disadvantages and power",
                "Words": [
                    {
                        "Word": "AI",
                        "Offset": 12800000,
                        "Duration": 800000
                    },
                    {
                        "Word": "enables",
                        "Offset": 13600000,
                        "Duration": 6800000
                    },
                    {
                        "Word": "us",
                        "Offset": 20400000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "to",
                        "Offset": 21600000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "build",
                        "Offset": 22800000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "amazing",
                        "Offset": 26000000,
                        "Duration": 6000000
                    },
                    {
                        "Word": "software",
                        "Offset": 32000000,
                        "Duration": 6400000
                    },
                    {
                        "Word": "that",
                        "Offset": 38400000,
                        "Duration": 1600000
                    },
                    {
                        "Word": "can",
                        "Offset": 40000000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "improve",
                        "Offset": 41200000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "health",
                        "Offset": 44400000,
                        "Duration": 2800000
                    },
                    {
                        "Word": "care",
                        "Offset": 47200000,
                        "Duration": 5200000
                    },
                    {
                        "Word": "enable",
                        "Offset": 55600000,
                        "Duration": 4000000
                    },
                    {
                        "Word": "people",
                        "Offset": 59600000,
                        "Duration": 3200000
                    },
                    {
                        "Word": "to",
                        "Offset": 62800000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "overcome",
                        "Offset": 64000000,
                        "Duration": 4800000
                    },
                    {
                        "Word": "physical",
                        "Offset": 68800000,
                        "Duration": 4000000
                    },
                    {
                        "Word": "disadvantages",
                        "Offset": 72800000,
                        "Duration": 12400000
                    },
                    {
                        "Word": "and",
                        "Offset": 88800000,
                        "Duration": 2000000
                    },
                    {
                        "Word": "power",
                        "Offset": 90800000,
                        "Duration": 4800000
                    }
                ]
            }
        ]
    },
    {
        "Id": "6508f1953c3e4439a877f1866558f1fc",
        "RecognitionStatus": 0,
        "Offset": 96000000,
        "Duration": 65200000,
        "Channel": 0,
        "DisplayText": "Empower smart infrastructure, create incredible entertainment experiences, and even save the planet.",
        "NBest": [
            {
                "Confidence": 0.8503038,
                "Lexical": "empower smart infrastructure create incredible entertainment experiences and even save the planet",
                "ITN": "empower smart infrastructure create incredible entertainment experiences and even save the planet",
                "MaskedITN": "empower smart infrastructure create incredible entertainment experiences and even save the planet",
                "Display": "Empower smart infrastructure, create incredible entertainment experiences, and even save the planet.",
                "Words": [
                    {
                        "Word": "empower",
                        "Offset": 96000000,
                        "Duration": 2800000
                    },
                    {
                        "Word": "smart",
                        "Offset": 98800000,
                        "Duration": 2000000
                    },
                    {
                        "Word": "infrastructure",
                        "Offset": 100800000,
                        "Duration": 5600000
                    },
                    {
                        "Word": "create",
                        "Offset": 109600000,
                        "Duration": 4400000
                    },
                    {
                        "Word": "incredible",
                        "Offset": 114000000,
                        "Duration": 6800000
                    },
                    {
                        "Word": "entertainment",
                        "Offset": 120800000,
                        "Duration": 6400000
                    },
                    {
                        "Word": "experiences",
                        "Offset": 127200000,
                        "Duration": 11200000
                    },
                    {
                        "Word": "and",
                        "Offset": 142400000,
                        "Duration": 2800000
                    },
                    {
                        "Word": "even",
                        "Offset": 145200000,
                        "Duration": 4400000
                    },
                    {
                        "Word": "save",
                        "Offset": 149600000,
                        "Duration": 3600000
                    },
                    {
                        "Word": "the",
                        "Offset": 153200000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "planet",
                        "Offset": 154400000,
                        "Duration": 6800000
                    }
                ]
            },
            {
                "Confidence": 0.7706533,
                "Lexical": "empower smart infrastructure creating incredible entertainment experiences and even save the planet",
                "ITN": "empower smart infrastructure creating incredible entertainment experiences and even save the planet",
                "MaskedITN": "empower smart infrastructure creating incredible entertainment experiences and even save the planet",
                "Display": "empower smart infrastructure creating incredible entertainment experiences and even save the planet",
                "Words": [
                    {
                        "Word": "empower",
                        "Offset": 96000000,
                        "Duration": 2800000
                    },
                    {
                        "Word": "smart",
                        "Offset": 98800000,
                        "Duration": 2000000
                    },
                    {
                        "Word": "infrastructure",
                        "Offset": 100800000,
                        "Duration": 5600000
                    },
                    {
                        "Word": "creating",
                        "Offset": 109600000,
                        "Duration": 6000000
                    },
                    {
                        "Word": "incredible",
                        "Offset": 115600000,
                        "Duration": 5200000
                    },
                    {
                        "Word": "entertainment",
                        "Offset": 120800000,
                        "Duration": 6400000
                    },
                    {
                        "Word": "experiences",
                        "Offset": 127200000,
                        "Duration": 11200000
                    },
                    {
                        "Word": "and",
                        "Offset": 142400000,
                        "Duration": 2800000
                    },
                    {
                        "Word": "even",
                        "Offset": 145200000,
                        "Duration": 4400000
                    },
                    {
                        "Word": "save",
                        "Offset": 149600000,
                        "Duration": 3600000
                    },
                    {
                        "Word": "the",
                        "Offset": 153200000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "planet",
                        "Offset": 154400000,
                        "Duration": 6800000
                    }
                ]
            },
            {
                "Confidence": 0.73178095,
                "Lexical": "empower smart infrastructure creating credible entertainment experiences and even save the planet",
                "ITN": "empower smart infrastructure creating credible entertainment experiences and even save the planet",
                "MaskedITN": "empower smart infrastructure creating credible entertainment experiences and even save the planet",
                "Display": "empower smart infrastructure creating credible entertainment experiences and even save the planet",
                "Words": [
                    {
                        "Word": "empower",
                        "Offset": 96000000,
                        "Duration": 2800000
                    },
                    {
                        "Word": "smart",
                        "Offset": 98800000,
                        "Duration": 2000000
                    },
                    {
                        "Word": "infrastructure",
                        "Offset": 100800000,
                        "Duration": 5600000
                    },
                    {
                        "Word": "creating",
                        "Offset": 109600000,
                        "Duration": 5600000
                    },
                    {
                        "Word": "credible",
                        "Offset": 115200000,
                        "Duration": 5600000
                    },
                    {
                        "Word": "entertainment",
                        "Offset": 120800000,
                        "Duration": 6400000
                    },
                    {
                        "Word": "experiences",
                        "Offset": 127200000,
                        "Duration": 11200000
                    },
                    {
                        "Word": "and",
                        "Offset": 142400000,
                        "Duration": 2800000
                    },
                    {
                        "Word": "even",
                        "Offset": 145200000,
                        "Duration": 4400000
                    },
                    {
                        "Word": "save",
                        "Offset": 149600000,
                        "Duration": 3600000
                    },
                    {
                        "Word": "the",
                        "Offset": 153200000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "planet",
                        "Offset": 154400000,
                        "Duration": 6800000
                    }
                ]
            },
            {
                "Confidence": 0.7791923,
                "Lexical": "empower smart infrastructure create incredible entertainment experiences and even save the planets",
                "ITN": "empower smart infrastructure create incredible entertainment experiences and even save the planets",
                "MaskedITN": "empower smart infrastructure create incredible entertainment experiences and even save the planets",
                "Display": "empower smart infrastructure create incredible entertainment experiences and even save the planets",
                "Words": [
                    {
                        "Word": "empower",
                        "Offset": 96000000,
                        "Duration": 2800000
                    },
                    {
                        "Word": "smart",
                        "Offset": 98800000,
                        "Duration": 2000000
                    },
                    {
                        "Word": "infrastructure",
                        "Offset": 100800000,
                        "Duration": 5600000
                    },
                    {
                        "Word": "create",
                        "Offset": 109600000,
                        "Duration": 4400000
                    },
                    {
                        "Word": "incredible",
                        "Offset": 114000000,
                        "Duration": 6800000
                    },
                    {
                        "Word": "entertainment",
                        "Offset": 120800000,
                        "Duration": 6400000
                    },
                    {
                        "Word": "experiences",
                        "Offset": 127200000,
                        "Duration": 11200000
                    },
                    {
                        "Word": "and",
                        "Offset": 142400000,
                        "Duration": 2800000
                    },
                    {
                        "Word": "even",
                        "Offset": 145200000,
                        "Duration": 4400000
                    },
                    {
                        "Word": "save",
                        "Offset": 149600000,
                        "Duration": 3600000
                    },
                    {
                        "Word": "the",
                        "Offset": 153200000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "planets",
                        "Offset": 154400000,
                        "Duration": 7200000
                    }
                ]
            },
            {
                "Confidence": 0.6995418,
                "Lexical": "empower smart infrastructure creating incredible entertainment experiences and even save the planets",
                "ITN": "empower smart infrastructure creating incredible entertainment experiences and even save the planets",
                "MaskedITN": "empower smart infrastructure creating incredible entertainment experiences and even save the planets",
                "Display": "empower smart infrastructure creating incredible entertainment experiences and even save the planets",
                "Words": [
                    {
                        "Word": "empower",
                        "Offset": 96000000,
                        "Duration": 2800000
                    },
                    {
                        "Word": "smart",
                        "Offset": 98800000,
                        "Duration": 2000000
                    },
                    {
                        "Word": "infrastructure",
                        "Offset": 100800000,
                        "Duration": 5600000
                    },
                    {
                        "Word": "creating",
                        "Offset": 109600000,
                        "Duration": 6000000
                    },
                    {
                        "Word": "incredible",
                        "Offset": 115600000,
                        "Duration": 5200000
                    },
                    {
                        "Word": "entertainment",
                        "Offset": 120800000,
                        "Duration": 6400000
                    },
                    {
                        "Word": "experiences",
                        "Offset": 127200000,
                        "Duration": 11200000
                    },
                    {
                        "Word": "and",
                        "Offset": 142400000,
                        "Duration": 2800000
                    },
                    {
                        "Word": "even",
                        "Offset": 145200000,
                        "Duration": 4400000
                    },
                    {
                        "Word": "save",
                        "Offset": 149600000,
                        "Duration": 3600000
                    },
                    {
                        "Word": "the",
                        "Offset": 153200000,
                        "Duration": 1200000
                    },
                    {
                        "Word": "planets",
                        "Offset": 154400000,
                        "Duration": 7200000
                    }
                ]
            }
        ]
    }
]
```
</details>


## Analyze text with Language Studio

Neste exercício, foi explorarado os recursos da Linguagem de IA do Azure analisando alguns exemplos de avaliações de hotéis. Utilizado o Language Studio para entender se as avaliações são majoritariamente positivas ou negativas.

O Processamento de Linguagem Natural (PNL) é um ramo da IA que lida com a linguagem escrita e falada. Podemos usar a PNL para criar soluções que extraem significado semântico do texto ou da fala ou que formulem respostas significativas em linguagem natural.

Por exemplo, suponha que a agente de viagens fictícia Margie's Travel incentive os clientes a enviar avaliações para estadias em hotéis. Pode-se usar o serviço Idioma para identificar frases-chave, determinar quais avaliações são positivas e quais são negativas ou analisar o texto de revisão em busca de menções a entidades conhecidas, como locais ou pessoas.

O Serviço de Linguagem de IA do Azure inclui análise de texto e recursos de PNL. Estes incluem a identificação de frases-chave no texto e a classificação do texto com base no sentimento.

### Execução

Foi selecionado o serviço "Analisar sentimento e minerar opiniões" (Analyze sentiment and mine opinions) na aba " Classificar texto" (Classify text).

Usamos o texto de exemplo do laboratório para ser analisado:

" Tired hotel with poor service
 The Royal Hotel, London, United Kingdom
 5/6/2018
 This is an old hotel (has been around since 1950's) and the room furnishings are average - becoming a bit old now and require changing. The internet didn't work and had to come to one of their office rooms to check in for my flight home. The website says it's close to the British Museum, but it's too far to walk."

Após clicar em RUN foi obtido a seguinte análise:

<img src="/LAB03 - Processamento de Linguagem Natural/inputs/SentimentAndOpinionMiningTryout.jpg" /> 

Observe que há um sentimento geral seguido de pontuações ao lado de três categorias, pontuação positiva, pontuação neutra, pontuação negativa. Em cada uma das categorias, é fornecida uma pontuação entre 0 e 1. Essas pontuações de confiança indicam a probabilidade de o texto fornecido ser um sentimento particular.

<details>
  <summary>Clique para exibir/ocultar o JSON</summary>
  
```json
{
    "documents": [
        {
            "id": "id__598",
            "sentiment": "negative",
            "confidenceScores": {
                "positive": 0,
                "neutral": 0.03,
                "negative": 0.96
            },
            "sentences": [
                {
                    "sentiment": "negative",
                    "confidenceScores": {
                        "positive": 0,
                        "neutral": 0.01,
                        "negative": 0.98
                    },
                    "offset": 0,
                    "length": 219,
                    "text": " Tired hotel with poor service  The Royal Hotel, London, United Kingdom  5/6/2018  This is an old hotel (has been around since 1950's) and the room furnishings are average - becoming a bit old now and require changing. ",
                    "targets": [
                        {
                            "sentiment": "negative",
                            "confidenceScores": {
                                "positive": 0.01,
                                "negative": 0.99
                            },
                            "offset": 7,
                            "length": 5,
                            "text": "hotel",
                            "relations": [
                                {
                                    "relationType": "assessment",
                                    "ref": "#/documents/0/sentences/0/assessments/0"
                                }
                            ]
                        },
                        {
                            "sentiment": "negative",
                            "confidenceScores": {
                                "positive": 0.01,
                                "negative": 0.99
                            },
                            "offset": 23,
                            "length": 7,
                            "text": "service",
                            "relations": [
                                {
                                    "relationType": "assessment",
                                    "ref": "#/documents/0/sentences/0/assessments/1"
                                }
                            ]
                        }
                    ],
                    "assessments": [
                        {
                            "sentiment": "negative",
                            "confidenceScores": {
                                "positive": 0.01,
                                "negative": 0.99
                            },
                            "offset": 1,
                            "length": 5,
                            "text": "Tired",
                            "isNegated": false
                        },
                        {
                            "sentiment": "negative",
                            "confidenceScores": {
                                "positive": 0.01,
                                "negative": 0.99
                            },
                            "offset": 18,
                            "length": 4,
                            "text": "poor",
                            "isNegated": false
                        }
                    ]
                },
                {
                    "sentiment": "negative",
                    "confidenceScores": {
                        "positive": 0,
                        "neutral": 0.01,
                        "negative": 0.99
                    },
                    "offset": 219,
                    "length": 102,
                    "text": "The internet didn't work and had to come to one of their office rooms to check in for my flight home. ",
                    "targets": [
                        {
                            "sentiment": "negative",
                            "confidenceScores": {
                                "positive": 0,
                                "negative": 1
                            },
                            "offset": 223,
                            "length": 8,
                            "text": "internet",
                            "relations": [
                                {
                                    "relationType": "assessment",
                                    "ref": "#/documents/0/sentences/1/assessments/0"
                                }
                            ]
                        }
                    ],
                    "assessments": [
                        {
                            "sentiment": "negative",
                            "confidenceScores": {
                                "positive": 0,
                                "negative": 1
                            },
                            "offset": 239,
                            "length": 4,
                            "text": "work",
                            "isNegated": true
                        }
                    ]
                },
                {
                    "sentiment": "negative",
                    "confidenceScores": {
                        "positive": 0.01,
                        "neutral": 0.08,
                        "negative": 0.91
                    },
                    "offset": 321,
                    "length": 76,
                    "text": "The website says it's close to the British Museum, but it's too far to walk.",
                    "targets": [],
                    "assessments": []
                }
            ],
            "warnings": []
        }
    ],
    "errors": [],
    "modelVersion": "2022-11-01"
}
```
</details>

## Referência

 - [Explore Speech Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/09-speech.html)
 - [Analyze text with Language Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-analysis.html)