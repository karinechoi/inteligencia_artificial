# Classificador de Lixo Reciclável
Universidade Presbiteriana Mackenzie
Faculdade de Computação e Informática – 2025
Projeto 1

## Membros
Aline Y. Higa – 10402138
Gustavo G. Munhoz – 10409258
Karine Y. Lim Choi – 10403237
Paula A. Oliveira – 10403270

## Descrição do Projeto
O projeto tem como objetivo automatizar a identificação e separação de materiais recicláveis, contribuindo para a sustentabilidade. O sistema deve ser capaz de reconhecer diferentes tipos de resíduos, como plástico, papel, vidro, orgânico, metal e não-recicláveis, por meio de imagens capturadas por câmeras, por um app mobile, por exemplo. A solução pode ser aplicada em centros de reciclagem, lixeiras inteligentes e processos industriais, otimizando o tempo e reduzindo custos operacionais. A inovação do projeto consiste em identificar, em uma única captura, vários objetos diferentes e classificá-los de acordo com as opções supracitadas. O projeto busca incentivar a reciclagem, diminuir o impacto ambiental do descarte inadequado e promover uma economia circular. Além disso, o projeto pode ser expandido para reconhecer materiais não recicláveis, aumentando a eficiência do gerenciamento de resíduos sólidos.

## Dataset TACO
​O TACO (Trash Annotations in Context) é um conjunto de dados de código aberto que contém imagens de resíduos sólidos em ambientes reais, como florestas, estradas e praias. As imagens são anotadas manualmente e segmentadas de acordo com uma taxonomia hierárquica, permitindo o treinamento e a avaliação de algoritmos de detecção de objetos. As anotações são fornecidas no formato COCO.
https://github.com/pedropro/TACO

## A análise exploratória
Conduzida no notebook Trabi.ipynb, contendo todo o processo de leitura, agrupamento e organização dos dados do dataset TACO. A primeira etapa consistiu no carregamento do arquivo original annotations.json, que contém as anotações completas do dataset. Esse arquivo foi clonado diretamente do repositório oficial do TACO ([[GitHub - TACO Dataset](http://tacodataset.org/)](https://github.com/pedropro/TACO)).

Etapas principais:
- Leitura do annotations.json original
- Mapeamento de subclasses específicas para macrogrupos de resíduos
- Criação de uma versão modificada do JSON com os novos rótulos (residuo_tipo)
- Separação inicial por tipo de material para fins de balanceamento futuro

