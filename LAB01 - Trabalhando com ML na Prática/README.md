
# Trabalhando com o Machine Learning na Prática no Azure ML

Neste exercício, foi utilizado o recurso de aprendizado de máquina automatizado no Aprendizado de Máquina do Azure para treinar e avaliar um modelo de aprendizado de máquina. Em seguida, foi implementado e testado o modelo treinado.

Para isso foi utilizado um laboratório cujo link está presente na sessão "Referência" deste documento.

O laboratório propõe um conjunto de dados de detalhes históricos de aluguel de bicicletas para treinar um modelo que prevê o número de aluguéis de bicicletas que devem ser esperados em um determinado dia, com base em características sazonais e meteorológicas.


## Publicação e Teste do Serviço

Após seguir os seguintes passos do laboratório...

    1. Criar um espaço de trabalho do Aprendizado de Máquina do Azure
    2. Usar o aprendizado de máquina automatizado para treinar um modelo
    3. Reveja o melhor modelo
    4. Implantar e testar o modelo

...foi realizada a etapa final "5. Testar o serviço implantado", cuja a entrada para testar o ponto de extremidade foi esse json sugerido: 

```json
 {
   "Inputs": { 
     "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]    
   },   
   "GlobalParameters": 1.0
 }
```
Na análise dos resultados do teste, que incluem um número previsto de aluguéis com base nos recursos de entrada:

```json
{
  "Results": [
    360.3462491961059
  ]
}
```
## Referência

 - [Explore Automated Machine Learning in Azure Machine Learning](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html)

