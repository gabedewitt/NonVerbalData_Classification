# NonVerbalData_Classification
![Badge Python](https://img.shields.io/badge/-Python-black?style=flat-square&logo=Python&logoColor=yellow)
![Jupyter](https://img.shields.io/badge/-Jupyter-black?style=flat-square&logo=Jupyter&logoColor=orange)
![Google Colab](https://img.shields.io/badge/-Google_Colab-black?style=flat-square&logo=Google+Colab&logoColor=orange)

## Contexto

Este projeto foi desenvolvido como etapa final do Programa de Formação de Dados das Lojas Renner S.A, com parceria da Cesar School. No programa foram ministradas aulas da linguagem de programação Python, aulas que lidaram com o controle de versionamento de software usando Git, Design Thinking, Design Sprint e, finalmente algoritmos de aprendizado de máquina, tanto Supervisionados quanto Não Supervisionado.

## O projeto

Nesse projeto utilizou-se a plataforma do Google Colab para carregar os dados do dataset de dados não verbais de turistas, ![disponível no repositório da univesidade de Irvine](https://archive.ics.uci.edu/ml/datasets/Non+verbal+tourists+data), e foram utilizadas duas estratégias de pré-processamento de dados para a comparação da performance da classificação com o uso do algoritmo K vizinhos mais próximos (KNN), a primeira utilizou a função get_dummies para converter os dados categóricos em numéricos, enquanto a segunda fez uso de label encoding.

## Resultados
<p align="center">
<img src="https://user-images.githubusercontent.com/51098239/172722027-3179ffc6-80d4-4785-9f76-9fe4b1c13ac4.png" alt="Gráfico dummies" width="650"/>
<img src="https://user-images.githubusercontent.com/51098239/172722042-a77e87ac-f54d-4a12-93ef-6963cf260ce9.png" alt="Gráfico label encoding" width="650"/>
</p>


Os resultados obtidos demonstraram que a função get_dummies, para esse dataset, apresentou performance melhor ao label encoding. Contudo, seria interessante realizar testes combinando ambas técnicas, pois segundo a descrição dos dados algumas colunas apresentam dados de caráter ordinal.

<p align="center">
<img src="https://user-images.githubusercontent.com/51098239/172722364-249fdf10-8612-403c-9b5c-8b1ba72f16b3.png" alt="Resultados do modelo"/>
<img src="https://user-images.githubusercontent.com/51098239/172722443-e8900c32-5a3a-4f9b-b16d-bac756a4af8c.png" alt="Matriz de Confusão"/>
</p>
  
Todavia, apesar desse resultado, também notou-se que há um desbalanceamento de classes nos dados e seria necessários ou a coleta de mais dados ou a adoção de uma técnica que equilibre as classes. Muito provavelmente um undersampling, visto que existem poucos registros e a replicação do oversampling pode descaracterizar os dados e enviesar o modelo de classificação.


 
