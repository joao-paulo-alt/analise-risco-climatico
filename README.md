# Análise de Dados Pluviométricos e Predição de Enchentes em Encantado/RS
![Imagem do projeto](https://th.bing.com/th/id/R.ac134a956faa4f11701812f2d4da86b5?rik=3c00S1MQyjke9g&riu=http%3a%2f%2ffolhapopular.info%2fwp-content%2fuploads%2f2020%2f07%2fWhatsApp-Image-2020-07-08-at-13.52.12.jpeg&ehk=Ff5LlfLksX%2bZrMif4hLuify22yAmbL%2fhI3DZItWEv1A%3d&risl=&pid=ImgRaw&r=0)

Este projeto examina os padrões de precipitação e níveis fluviais no município de Encantado/RS, desenvolvendo um modelo preditivo para risco de enchentes. A análise é baseada em dados históricos de chuva e níveis do rio Taquari, oferecendo insights valiosos para gestão de desastres naturais.

## Os Dados Pluviométricos de Encantado
As variáveis de precipitação (volumes diários, mensais e anuais) e nível do rio são características críticas para prever eventos extremos. Esses dados foram coletados sistematicamente, permitindo análises temporais e preditivas.

## Desenvolvedor
João Paulo Ferreira (https://github.com/joao-paulo-alt)

## Justificativa
Estudos sobre padrões pluviométricos e hidrológicos são essenciais para:
- Mitigar os impactos de eventos climáticos extremos
- Melhorar sistemas de alerta precoce
- Planejar ações de defesa civil
- Entender as relações entre precipitação e níveis fluviais

Este projeto aborda questões fundamentais:
- Quais os padrões sazonais de precipitação na região?
- Como as variáveis pluviométricas se correlacionam com o nível do rio?
- É possível prever eventos de risco com antecedência?

## Estrutura dos Dados
As principais variáveis analisadas incluem:
- **Variáveis temporais**: Data, Ano, Mês, Estação
- **Dados pluviométricos**: 
  - Precipitação diária máxima (mm)
  - Volume mensal (mm)
  - Dias chuvosos
- **Variáveis fluviais**: Nível do rio (m)
- **Variável alvo**: Risco de enchente (binário)

## Estrutura do Projeto
analise-alertaviva/
├── dados/
│   ├── encantado-annual-rainfall.csv
│   ├── encantado-rain-data.csv
│   ├── encantado-rain-flood.csv
│   ├── dados-merged-data.csv
├── notebooks/
│   ├── 1_preprocessamento.ipynb
│   ├── 2_limpeza_dados.ipynb
│   ├── 3_analise_exploratoria.ipynb
│   └── 4_modelagem.ipynb
└── README.md

## Metodologia
O projeto foi desenvolvido seguindo a metodologia CRISP-DM:
1. Entendimento do problema
2. Coleta e preparação dos dados
3. Análise exploratória
4. Modelagem preditiva
5. Avaliação e validação

## Resultados Obtidos
O projeto alcançou os seguintes resultados:
- Identificação de padrões sazonais (maior precipitação no inverno)
- Desenvolvimento de modelo preditivo com 99% de acurácia
- Determinação das variáveis mais importantes para risco de enchente:
  1. Nível do rio (49% de importância)
  2. Precipitação diária máxima (25%)
  3. Precipitação mensal (10%)

## Recursos Técnicos
- Linguagem: Python
- Bibliotecas principais: Pandas, Scikit-learn, Matplotlib/Seaborn
- Algoritmo: Random Forest
- Validação: Cross-validation (5 folds)

## Licença
MIT License