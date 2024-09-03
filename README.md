# Pacote de Processamento de Imagens

Este repositório fornece um pacote Python para o processamento de imagens. O pacote inclui funcionalidades para comparar, transformar e visualizar imagens de forma simples e eficiente.

## Descrição

Este pacote oferece ferramentas úteis para processamento de imagens, como comparação de imagens, transformação e visualização. Ideal para quem trabalha com análise de imagens e precisa de um conjunto de funções básicas.

## Instalação

Para instalar o pacote, você pode usar pip:

```bash
pip install image-processing-package
```

## Pré-requisitos
- Python 3.8 ou superior
- pip

## Como Usar (Usuários)
### Testando os módulos:
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

## Como Usar (Desenvolvedores/Colaboradores)
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
4. Gerar os binários para publicação:
```bash
python -m pip install --upgrade pip
python -m pip install twine setuptools wheel

python setup.py sdist bdist_wheel
```

## CheckList para publicação

 - [ ] Criar conta no [Test Pypi](https://test.pypi.org/account/register/)
 - [ ] Publicar no Test Pypi
 - [ ] Instalar pacote usando Test Pypi
 - [ ] Testar pacote
 - [ ] Criar conta no [Pypi](https://pypi.org/account/register/)
 - [ ] Publicar no Pypi
 - [ ] Instalar pacote usando Pypi


## Créditos
<table>
  <tr>
    <td align="center">
      <a href="https://github.com/tiemi/">
        <img src="https://github.com/tiemi.png" width="110px" alt=""/><br>
        <sub>
          <b>Tiemi</b>
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/digitalinnovationone/">
        <img src="https://github.com/digitalinnovationone.png" width="110px" alt=""/><br>
        <sub>
          <b>DIO</b>
        </sub>
      </a>
    </td>
  </tr>
</table>

## Licença
Veja [MIT](https://choosealicense.com/licenses/mit/) para mais detalhes.