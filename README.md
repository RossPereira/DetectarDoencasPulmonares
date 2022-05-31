# Cenário e Solução:

**Cenário:** Graças ao avanço dos algoritmos de machine learning e deep learning coisas que antes eram impensáveis hoje podem ser automatizadas, hoje trarei um grande exemplo disso: O caso desse projeto em que através de imagens de raio-x podemos pré-diagnosticar doenças pulmonares com uma grande taxa de acerto e assim tornar mais rápido e preciso a avaliação médica posterior.

**Solução proposta:** Será usada uma rede neural convolucional que explicando a grosso modo recebe a imagem, as camadas internas da rede extraem caracteristicas dessas imagens e passam essas caracteristicas para a camada de saída responsável por classificar entre as 4 categorias estabelecidas acima

# Bibliotecas Usadas:

* Tensorflow
* Keras
* Scikit learn
* OpenCV
* Numpy
* Seaborn
* MatPlotLib

# Técnicas de Machine Learning:
* Deep Learning
* Transferência de aprendizagem: Rede Resnet
* Divisão de dados: Holdout


# Construção:

Foi usada uma rede neural convolucional que recebeu grande parte da sua arquitetura atráves de um rede neural maior já treinada chamada de Resnet através de transferência de aprendizagem. A Resnet é uma arquitetura de rede neural que foi treinada com uma base de 11 milhoes de imagens chamada imagenet.

Como base de dados possuíamos um banco de imagens de raio-x dividido em 4 classe sendo: 0-Covid19, 1-Pessoas sem nenhuma doença, 2-Pneumonia Viral, 3-Pneumonia Bacteriana. a Camada de entrada e as camadas ocultas foram transferidas da Resnet, a camada de saída foi personalizada. Ao final do treinamento o modelo alcançou uma acurácia de 82%. 

