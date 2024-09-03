# package_name

Description.
The package package_name is used to:
-

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install package_name

```bash
pip install package_name
```

## Usage

```python
from package_name.module1_name import file1_name
file1_name.my_function()
```

## Author
My_name

## License
[MIT](https://choosealicense.com/licenses/mit/)






# Pacote de Processamento de Imagens

Este repositório fornece um pacote Python para o processamento de imagens. O pacote inclui funcionalidades para comparar, transformar e visualizar imagens de forma simples e eficiente.

## Descrição

Este pacote oferece ferramentas úteis para processamento de imagens, como comparação de imagens, transformação e visualização. Ideal para quem trabalha com análise de imagens e precisa de um conjunto de funções básicas.

## 📦 Instalação

Para instalar o pacote, você pode usar pip:

```bash
pip install image-processing-package
```

## 📋 Pré-requisitos
- Python 3.8 ou superior
- pip

## 🛠️ Como Usar
1. Clone o repositório:
```bash
git clone https://github.com/rafael-vas/image-processing-package.git
```
2. Navegue até o diretório do projeto:
```bash
cd image-processing-package
```
3. Instale as dependências:
```bash
pip install -r requirements.txt
```

4. Testando os módulos:
```python
from image_processing.processing.combination import find_difference

image1 = # carregar a primeira imagem
image2 = # carregar a segunda imagem

difference_image = find_difference(image1, image2)
```

```python
from image_processing.processing.transformation import resize_image

image = # carregar a imagem
resized_image = resize_image(image, proportion=0.5)
```

```python
from image_processing.utils.io import read_image, save_image

image = read_image('caminho/para/imagem.jpg')
save_image(image, 'caminho/para/salvar_imagem.jpg')
```

```python
from image_processing.utils.plot import plot_image, plot_result, plot_histogram

plot_image(image)
plot_result(image1, image2, difference_image)
plot_histogram(image)
```

## Gerar binários para publicar
Para gerar os binários
```bash
python -m pip install --upgrade pip
python -m pip install twine
python -m pip install setuptools
python -m pip install wheel

python setup.py sdist bdist_wheel
```

## Licença
Veja [MIT](https://choosealicense.com/licenses/mit/) para mais detalhes.