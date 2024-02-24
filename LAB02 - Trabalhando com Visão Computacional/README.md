
# Reconhecimento Facial e transformação de imagens em Dados no Azure ML

Neste exercício, foi utilizado o Portal Vision Cognitive do Azure para detecção de rostos em uma imagem, extrair textos de imagens e adicionar legendas a imagens.

O laboratório propõe experimentar alguns dos serviços Azure relacionado a Visão Computacional.

## Detecção de rostos em uma imagem

Detecte a localização de um ou mais rostos humanos em imagens, juntamente com atributos como pose, máscara facial e pontos de referência faciais.


<img src="/workspaces/Microsoft-Azure-AI/LAB02 - Trabalhando com Visão Computacional/outputs/01-Processada.jpg" /> 

<details>
  <summary>Clique para exibir/ocultar o JSON</summary>
  
```json

[
  {
    "recognitionModel": "recognition_01",
    "faceRectangle": {
      "width": 148,
      "height": 224,
      "left": 105,
      "top": 43
    },
    "faceLandmarks": {
      "pupilLeft": {
        "x": 140.2,
        "y": 144.6
      },
      "pupilRight": {
        "x": 211.5,
        "y": 143.8
      },
      "noseTip": {
        "x": 172.2,
        "y": 180.2
      },
      "mouthLeft": {
        "x": 147.2,
        "y": 216.7
      },
      "mouthRight": {
        "x": 205.8,
        "y": 215
      },
      "eyebrowLeftOuter": {
        "x": 120.3,
        "y": 127.7
      },
      "eyebrowLeftInner": {
        "x": 154.6,
        "y": 127.1
      },
      "eyeLeftOuter": {
        "x": 127.4,
        "y": 145.2
      },
      "eyeLeftTop": {
        "x": 141.6,
        "y": 139.6
      },
      "eyeLeftBottom": {
        "x": 138.3,
        "y": 148.4
      },
      "eyeLeftInner": {
        "x": 153.3,
        "y": 145.1
      },
      "eyebrowRightInner": {
        "x": 191.1,
        "y": 128.3
      },
      "eyebrowRightOuter": {
        "x": 234.1,
        "y": 131.4
      },
      "eyeRightInner": {
        "x": 198.6,
        "y": 145
      },
      "eyeRightTop": {
        "x": 209.9,
        "y": 138.3
      },
      "eyeRightBottom": {
        "x": 212.3,
        "y": 147.7
      },
      "eyeRightOuter": {
        "x": 225.2,
        "y": 144
      },
      "noseRootLeft": {
        "x": 163.4,
        "y": 148.6
      },
      "noseRootRight": {
        "x": 184,
        "y": 147.9
      },
      "noseLeftAlarTop": {
        "x": 158,
        "y": 172.1
      },
      "noseRightAlarTop": {
        "x": 189.4,
        "y": 171
      },
      "noseLeftAlarOutTip": {
        "x": 153,
        "y": 186.1
      },
      "noseRightAlarOutTip": {
        "x": 195.7,
        "y": 186
      },
      "upperLipTop": {
        "x": 176.9,
        "y": 212.5
      },
      "upperLipBottom": {
        "x": 175.4,
        "y": 216.6
      },
      "underLipTop": {
        "x": 175.2,
        "y": 218.4
      },
      "underLipBottom": {
        "x": 175.8,
        "y": 225.1
      }
    },
    "faceAttributes": {
      "mask": {
        "type": "noMask",
        "noseAndMouthCovered": false
      }
    }
  }
]

```

</details>

## Extrair textos de imagens

Use a API de leitura para extrair texto impresso e manuscrito em idiomas com suporte de imagens, PDFs e arquivos TIFF. O recurso de reconhecimento óptico de caracteres (OCR) oferece suporte a imagens e documentos com idiomas mistos e não requer a especificação do idioma.


<img src="/workspaces/Microsoft-Azure-AI/LAB02 - Trabalhando com Visão Computacional/outputs/02-Processada.jpg" /> 


<details>
  <summary>Clique para exibir/ocultar o JSON</summary>

```json
[
  {
    "lines": [
      {
        "text": "CERTIFICADO",
        "boundingPolygon": [
          {
            "x": 137,
            "y": 42
          },
          {
            "x": 484,
            "y": 42
          },
          {
            "x": 484,
            "y": 82
          },
          {
            "x": 137,
            "y": 81
          }
        ],
        "words": [
          {
            "text": "CERTIFICADO",
            "boundingPolygon": [
              {
                "x": 138,
                "y": 43
              },
              {
                "x": 464,
                "y": 43
              },
              {
                "x": 465,
                "y": 82
              },
              {
                "x": 138,
                "y": 83
              }
            ],
            "confidence": 0.993
          }
        ]
      },
      {
        "text": "de Voluntariado",
        "boundingPolygon": [
          {
            "x": 237,
            "y": 95
          },
          {
            "x": 385,
            "y": 95
          },
          {
            "x": 385,
            "y": 113
          },
          {
            "x": 237,
            "y": 113
          }
        ],
        "words": [
          {
            "text": "de",
            "boundingPolygon": [
              {
                "x": 238,
                "y": 96
              },
              {
                "x": 259,
                "y": 96
              },
              {
                "x": 259,
                "y": 113
              },
              {
                "x": 238,
                "y": 113
              }
            ],
            "confidence": 0.999
          },
          {
            "text": "Voluntariado",
            "boundingPolygon": [
              {
                "x": 266,
                "y": 96
              },
              {
                "x": 381,
                "y": 96
              },
              {
                "x": 381,
                "y": 113
              },
              {
                "x": 266,
                "y": 113
              }
            ],
            "confidence": 0.993
          }
        ]
      },
      {
        "text": "Conferimos a",
        "boundingPolygon": [
          {
            "x": 268,
            "y": 132
          },
          {
            "x": 354,
            "y": 132
          },
          {
            "x": 354,
            "y": 145
          },
          {
            "x": 268,
            "y": 145
          }
        ],
        "words": [
          {
            "text": "Conferimos",
            "boundingPolygon": [
              {
                "x": 270,
                "y": 132
              },
              {
                "x": 342,
                "y": 133
              },
              {
                "x": 342,
                "y": 145
              },
              {
                "x": 270,
                "y": 146
              }
            ],
            "confidence": 0.994
          },
          {
            "text": "a",
            "boundingPolygon": [
              {
                "x": 346,
                "y": 133
              },
              {
                "x": 352,
                "y": 133
              },
              {
                "x": 352,
                "y": 145
              },
              {
                "x": 346,
                "y": 145
              }
            ],
            "confidence": 0.994
          }
        ]
      },
      {
        "text": "Fernando Claudiano Maia",
        "boundingPolygon": [
          {
            "x": 171,
            "y": 155
          },
          {
            "x": 450,
            "y": 155
          },
          {
            "x": 450,
            "y": 176
          },
          {
            "x": 171,
            "y": 177
          }
        ],
        "words": [
          {
            "text": "Fernando",
            "boundingPolygon": [
              {
                "x": 172,
                "y": 156
              },
              {
                "x": 273,
                "y": 155
              },
              {
                "x": 273,
                "y": 177
              },
              {
                "x": 171,
                "y": 178
              }
            ],
            "confidence": 0.995
          },
          {
            "text": "Claudiano",
            "boundingPolygon": [
              {
                "x": 282,
                "y": 155
              },
              {
                "x": 389,
                "y": 155
              },
              {
                "x": 388,
                "y": 177
              },
              {
                "x": 281,
                "y": 177
              }
            ],
            "confidence": 0.993
          },
          {
            "text": "Maia",
            "boundingPolygon": [
              {
                "x": 398,
                "y": 155
              },
              {
                "x": 448,
                "y": 156
              },
              {
                "x": 448,
                "y": 176
              },
              {
                "x": 397,
                "y": 177
              }
            ],
            "confidence": 0.992
          }
        ]
      },
      {
        "text": "em reconhecimento pela atuação em prol da formação das",
        "boundingPolygon": [
          {
            "x": 136,
            "y": 191
          },
          {
            "x": 484,
            "y": 191
          },
          {
            "x": 484,
            "y": 206
          },
          {
            "x": 136,
            "y": 205
          }
        ],
        "words": [
          {
            "text": "em",
            "boundingPolygon": [
              {
                "x": 138,
                "y": 192
              },
              {
                "x": 152,
                "y": 192
              },
              {
                "x": 152,
                "y": 206
              },
              {
                "x": 138,
                "y": 206
              }
            ],
            "confidence": 0.999
          },
          {
            "text": "reconhecimento",
            "boundingPolygon": [
              {
                "x": 160,
                "y": 192
              },
              {
                "x": 257,
                "y": 191
              },
              {
                "x": 256,
                "y": 206
              },
              {
                "x": 159,
                "y": 206
              }
            ],
            "confidence": 0.994
          },
          {
            "text": "pela",
            "boundingPolygon": [
              {
                "x": 260,
                "y": 191
              },
              {
                "x": 284,
                "y": 191
              },
              {
                "x": 284,
                "y": 206
              },
              {
                "x": 259,
                "y": 206
              }
            ],
            "confidence": 0.993
          },
          {
            "text": "atuação",
            "boundingPolygon": [
              {
                "x": 287,
                "y": 191
              },
              {
                "x": 334,
                "y": 191
              },
              {
                "x": 334,
                "y": 206
              },
              {
                "x": 287,
                "y": 206
              }
            ],
            "confidence": 0.959
          },
          {
            "text": "em",
            "boundingPolygon": [
              {
                "x": 337,
                "y": 191
              },
              {
                "x": 352,
                "y": 191
              },
              {
                "x": 352,
                "y": 206
              },
              {
                "x": 337,
                "y": 206
              }
            ],
            "confidence": 0.999
          },
          {
            "text": "prol",
            "boundingPolygon": [
              {
                "x": 360,
                "y": 191
              },
              {
                "x": 382,
                "y": 191
              },
              {
                "x": 382,
                "y": 206
              },
              {
                "x": 359,
                "y": 206
              }
            ],
            "confidence": 0.992
          },
          {
            "text": "da",
            "boundingPolygon": [
              {
                "x": 385,
                "y": 191
              },
              {
                "x": 400,
                "y": 192
              },
              {
                "x": 400,
                "y": 206
              },
              {
                "x": 385,
                "y": 206
              }
            ],
            "confidence": 0.999
          },
          {
            "text": "formação",
            "boundingPolygon": [
              {
                "x": 403,
                "y": 192
              },
              {
                "x": 458,
                "y": 192
              },
              {
                "x": 458,
                "y": 206
              },
              {
                "x": 403,
                "y": 206
              }
            ],
            "confidence": 0.947
          },
          {
            "text": "das",
            "boundingPolygon": [
              {
                "x": 461,
                "y": 192
              },
              {
                "x": 484,
                "y": 192
              },
              {
                "x": 484,
                "y": 205
              },
              {
                "x": 461,
                "y": 205
              }
            ],
            "confidence": 0.999
          }
        ]
      },
      {
        "text": "juventudes por meio do programa Empresário Sombra Por",
        "boundingPolygon": [
          {
            "x": 136,
            "y": 207
          },
          {
            "x": 484,
            "y": 207
          },
          {
            "x": 484,
            "y": 221
          },
          {
            "x": 136,
            "y": 221
          }
        ],
        "words": [
          {
            "text": "juventudes",
            "boundingPolygon": [
              {
                "x": 136,
                "y": 207
              },
              {
                "x": 203,
                "y": 207
              },
              {
                "x": 203,
                "y": 222
              },
              {
                "x": 136,
                "y": 222
              }
            ],
            "confidence": 0.993
          },
          {
            "text": "por",
            "boundingPolygon": [
              {
                "x": 206,
                "y": 207
              },
              {
                "x": 227,
                "y": 207
              },
              {
                "x": 227,
                "y": 222
              },
              {
                "x": 206,
                "y": 222
              }
            ],
            "confidence": 0.993
          },
          {
            "text": "meio",
            "boundingPolygon": [
              {
                "x": 230,
                "y": 207
              },
              {
                "x": 260,
                "y": 207
              },
              {
                "x": 260,
                "y": 222
              },
              {
                "x": 230,
                "y": 222
              }
            ],
            "confidence": 0.991
          },
          {
            "text": "do",
            "boundingPolygon": [
              {
                "x": 263,
                "y": 207
              },
              {
                "x": 278,
                "y": 207
              },
              {
                "x": 278,
                "y": 222
              },
              {
                "x": 263,
                "y": 222
              }
            ],
            "confidence": 0.998
          },
          {
            "text": "programa",
            "boundingPolygon": [
              {
                "x": 281,
                "y": 207
              },
              {
                "x": 340,
                "y": 207
              },
              {
                "x": 340,
                "y": 221
              },
              {
                "x": 281,
                "y": 222
              }
            ],
            "confidence": 0.994
          },
          {
            "text": "Empresário",
            "boundingPolygon": [
              {
                "x": 343,
                "y": 207
              },
              {
                "x": 410,
                "y": 208
              },
              {
                "x": 409,
                "y": 221
              },
              {
                "x": 343,
                "y": 221
              }
            ],
            "confidence": 0.599
          },
          {
            "text": "Sombra",
            "boundingPolygon": [
              {
                "x": 413,
                "y": 208
              },
              {
                "x": 458,
                "y": 208
              },
              {
                "x": 458,
                "y": 221
              },
              {
                "x": 413,
                "y": 221
              }
            ],
            "confidence": 0.996
          },
          {
            "text": "Por",
            "boundingPolygon": [
              {
                "x": 462,
                "y": 208
              },
              {
                "x": 484,
                "y": 208
              },
              {
                "x": 483,
                "y": 221
              },
              {
                "x": 462,
                "y": 221
              }
            ],
            "confidence": 0.998
          }
        ]
      },
      {
        "text": "Um Dia com carga horária de 05h em 23/08/2023.",
        "boundingPolygon": [
          {
            "x": 137,
            "y": 222
          },
          {
            "x": 426,
            "y": 222
          },
          {
            "x": 426,
            "y": 236
          },
          {
            "x": 137,
            "y": 237
          }
        ],
        "words": [
          {
            "text": "Um",
            "boundingPolygon": [
              {
                "x": 138,
                "y": 223
              },
              {
                "x": 155,
                "y": 223
              },
              {
                "x": 154,
                "y": 237
              },
              {
                "x": 138,
                "y": 237
              }
            ],
            "confidence": 0.998
          },
          {
            "text": "Dia",
            "boundingPolygon": [
              {
                "x": 162,
                "y": 223
              },
              {
                "x": 181,
                "y": 223
              },
              {
                "x": 181,
                "y": 237
              },
              {
                "x": 162,
                "y": 237
              }
            ],
            "confidence": 0.998
          },
          {
            "text": "com",
            "boundingPolygon": [
              {
                "x": 184,
                "y": 223
              },
              {
                "x": 205,
                "y": 223
              },
              {
                "x": 205,
                "y": 237
              },
              {
                "x": 184,
                "y": 237
              }
            ],
            "confidence": 0.999
          },
          {
            "text": "carga",
            "boundingPolygon": [
              {
                "x": 214,
                "y": 223
              },
              {
                "x": 246,
                "y": 223
              },
              {
                "x": 245,
                "y": 237
              },
              {
                "x": 213,
                "y": 237
              }
            ],
            "confidence": 0.997
          },
          {
            "text": "horária",
            "boundingPolygon": [
              {
                "x": 249,
                "y": 223
              },
              {
                "x": 290,
                "y": 223
              },
              {
                "x": 290,
                "y": 237
              },
              {
                "x": 248,
                "y": 237
              }
            ],
            "confidence": 0.792
          },
          {
            "text": "de",
            "boundingPolygon": [
              {
                "x": 293,
                "y": 223
              },
              {
                "x": 308,
                "y": 223
              },
              {
                "x": 308,
                "y": 237
              },
              {
                "x": 292,
                "y": 237
              }
            ],
            "confidence": 0.993
          },
          {
            "text": "05h",
            "boundingPolygon": [
              {
                "x": 311,
                "y": 223
              },
              {
                "x": 332,
                "y": 223
              },
              {
                "x": 332,
                "y": 237
              },
              {
                "x": 311,
                "y": 237
              }
            ],
            "confidence": 0.993
          },
          {
            "text": "em",
            "boundingPolygon": [
              {
                "x": 336,
                "y": 223
              },
              {
                "x": 350,
                "y": 223
              },
              {
                "x": 350,
                "y": 237
              },
              {
                "x": 336,
                "y": 237
              }
            ],
            "confidence": 0.998
          },
          {
            "text": "23/08/2023.",
            "boundingPolygon": [
              {
                "x": 359,
                "y": 223
              },
              {
                "x": 426,
                "y": 223
              },
              {
                "x": 426,
                "y": 236
              },
              {
                "x": 359,
                "y": 237
              }
            ],
            "confidence": 0.991
          }
        ]
      },
      {
        "text": "Brenda Santos",
        "boundingPolygon": [
          {
            "x": 145,
            "y": 259
          },
          {
            "x": 256,
            "y": 259
          },
          {
            "x": 256,
            "y": 285
          },
          {
            "x": 145,
            "y": 285
          }
        ],
        "words": [
          {
            "text": "Brenda",
            "boundingPolygon": [
              {
                "x": 154,
                "y": 260
              },
              {
                "x": 205,
                "y": 261
              },
              {
                "x": 205,
                "y": 286
              },
              {
                "x": 153,
                "y": 286
              }
            ],
            "confidence": 0.941
          },
          {
            "text": "Santos",
            "boundingPolygon": [
              {
                "x": 210,
                "y": 261
              },
              {
                "x": 253,
                "y": 261
              },
              {
                "x": 253,
                "y": 286
              },
              {
                "x": 211,
                "y": 286
              }
            ],
            "confidence": 0.888
          }
        ]
      },
      {
        "text": "JA",
        "boundingPolygon": [
          {
            "x": 417,
            "y": 277
          },
          {
            "x": 431,
            "y": 277
          },
          {
            "x": 431,
            "y": 286
          },
          {
            "x": 417,
            "y": 286
          }
        ],
        "words": [
          {
            "text": "JA",
            "boundingPolygon": [
              {
                "x": 419,
                "y": 277
              },
              {
                "x": 430,
                "y": 277
              },
              {
                "x": 430,
                "y": 286
              },
              {
                "x": 419,
                "y": 286
              }
            ],
            "confidence": 0.917
          }
        ]
      },
      {
        "text": "Brenda Santos",
        "boundingPolygon": [
          {
            "x": 170,
            "y": 289
          },
          {
            "x": 230,
            "y": 290
          },
          {
            "x": 230,
            "y": 300
          },
          {
            "x": 170,
            "y": 299
          }
        ],
        "words": [
          {
            "text": "Brenda",
            "boundingPolygon": [
              {
                "x": 170,
                "y": 290
              },
              {
                "x": 199,
                "y": 290
              },
              {
                "x": 199,
                "y": 300
              },
              {
                "x": 170,
                "y": 300
              }
            ],
            "confidence": 0.991
          },
          {
            "text": "Santos",
            "boundingPolygon": [
              {
                "x": 201,
                "y": 290
              },
              {
                "x": 229,
                "y": 291
              },
              {
                "x": 229,
                "y": 300
              },
              {
                "x": 201,
                "y": 300
              }
            ],
            "confidence": 0.994
          }
        ]
      },
      {
        "text": "Brasil",
        "boundingPolygon": [
          {
            "x": 416,
            "y": 288
          },
          {
            "x": 449,
            "y": 288
          },
          {
            "x": 449,
            "y": 298
          },
          {
            "x": 416,
            "y": 298
          }
        ],
        "words": [
          {
            "text": "Brasil",
            "boundingPolygon": [
              {
                "x": 417,
                "y": 288
              },
              {
                "x": 449,
                "y": 289
              },
              {
                "x": 448,
                "y": 299
              },
              {
                "x": 417,
                "y": 299
              }
            ],
            "confidence": 0.995
          }
        ]
      },
      {
        "text": "Diretora de Operações",
        "boundingPolygon": [
          {
            "x": 153,
            "y": 300
          },
          {
            "x": 246,
            "y": 300
          },
          {
            "x": 246,
            "y": 311
          },
          {
            "x": 153,
            "y": 311
          }
        ],
        "words": [
          {
            "text": "Diretora",
            "boundingPolygon": [
              {
                "x": 154,
                "y": 301
              },
              {
                "x": 187,
                "y": 300
              },
              {
                "x": 186,
                "y": 312
              },
              {
                "x": 154,
                "y": 311
              }
            ],
            "confidence": 0.994
          },
          {
            "text": "de",
            "boundingPolygon": [
              {
                "x": 189,
                "y": 300
              },
              {
                "x": 199,
                "y": 300
              },
              {
                "x": 198,
                "y": 312
              },
              {
                "x": 189,
                "y": 312
              }
            ],
            "confidence": 0.998
          },
          {
            "text": "Operações",
            "boundingPolygon": [
              {
                "x": 201,
                "y": 300
              },
              {
                "x": 246,
                "y": 301
              },
              {
                "x": 245,
                "y": 311
              },
              {
                "x": 201,
                "y": 312
              }
            ],
            "confidence": 0.952
          }
        ]
      }
    ]
  }
]

```
</details>

## Adicionar legendas a imagens

Gere uma frase legível por humanos que descreva o conteúdo de uma imagem.


<img src="/workspaces/Microsoft-Azure-AI/LAB02 - Trabalhando com Visão Computacional/outputs/03-Processada.jpg" /> 

<details>
  <summary>Clique para exibir/ocultar o JSON</summary>
  
```json
{
  "apim-request-id": "e4f733af-fabd-4dc6-a48d-213d7456a05c",
  "content-length": "168",
  "content-type": "application/json; charset=utf-8",
  "modelVersion": "2023-10-01",
  "captionResult": {
    "text": "cartoon character with cartoon characters",
    "confidence": 0.6841980814933777
  },
  "metadata": {
    "width": 234,
    "height": 215
  }
}
```
</details>