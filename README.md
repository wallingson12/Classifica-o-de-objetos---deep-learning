# Classificação de Imagens de Laranjas com Rede Neural Convolucional

Este projeto utiliza uma rede neural convolucional (CNN) para classificar imagens de laranjas e não laranjas. O código realiza as seguintes etapas:

1. Carregamento e pré-processamento das imagens.
2. Criação de labels para as imagens (laranja ou não laranja).
3. Divisão do conjunto de dados em treinamento e validação.
4. Normalização dos dados.
5. Aumento de dados (data augmentation) para melhorar a generalização do modelo.
6. Definição e treinamento do modelo CNN.
7. Avaliação do modelo.
8. Salvamento do modelo treinado.
9. Predição de novas imagens.

## Estrutura do Projeto

- `load_images_from_folder(folder_path, image_size=(128, 128))`: Função para carregar e pré-processar imagens de um diretório.
- `load_and_preprocess_image(image_path, image_size=(128, 128))`: Função para carregar e pré-processar uma imagem específica.
- Caminhos dos diretórios das imagens de treinamento: `laranja_folder_path` e `not_laranja_folder_path`.
- Criação de labels e combinação dos dados.
- Divisão do conjunto de dados em `X_train`, `X_val`, `y_train` e `y_val`.
- Normalização dos dados.
- Definição do `ImageDataGenerator` para data augmentation.
- Definição do modelo CNN utilizando `tf.keras.Sequential`.
- Compilação e treinamento do modelo.
- Salvamento do modelo treinado em `saved_model.h5`.
- Função `predict_image(model, image_path)` para fazer predições em novas imagens.

## Requisitos

- Python 3.x
- OpenCV
- NumPy
- TensorFlow
- Scikit-learn
- Matplotlib
