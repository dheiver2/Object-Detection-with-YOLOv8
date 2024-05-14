
# Detector de Objetos com YOLO

Este script é uma ferramenta versátil para detecção de objetos em imagens, vídeos, streams ao vivo e vídeos do YouTube usando o modelo YOLO (You Only Look Once).

## Funcionalidades

- Processamento de imagens estáticas (JPEG, PNG)
- Processamento de vídeos (MP4)
- Detecção em imagens via URL HTTP
- Captura de tela do monitor
- Transmissão ao vivo de webcam
- Transmissão ao vivo de URLs de streaming
- Reprodução de vídeos do YouTube
- Processamento em lote de imagens em um diretório
- Suporte para múltiplos fluxos de vídeo

## Instalação

Para utilizar este script, é necessário instalar as seguintes dependências:

- Python 3.x
- numpy
- supervision
- ultralytics
- requests
- Pillow
- opencv-python
- torch
- pandas
- mss
- pafy

Você pode instalar essas dependências via pip:

```
pip install -r requirements.txt
```

## Uso

Você pode executar o script fornecendo diferentes tipos de entrada. Aqui estão alguns exemplos:

- Processar uma imagem estática:

```
python main.py /caminho/para/imagem.jpg
```

- Processar um vídeo:

```
python main.py /caminho/para/video.mp4
```

- Processar uma imagem via URL HTTP:

```
python main.py http://exemplo.com/caminho/para/imagem.jpg
```

- Capturar e processar uma tela do monitor:

```
python main.py screen
```

- Transmitir ao vivo da webcam:

```
python main.py webcam
```

- Reproduzir um vídeo do YouTube:

```
python main.py https://youtu.be/LNwODJXcvt4
```

- Processar um diretório de imagens em lote:

```
python main.py /caminho/para/diretorio
```

- Processar múltiplos fluxos de vídeo listados em um arquivo:

```
python main.py /caminho/para/lista_de_fluxos.streams
```

Consulte o arquivo `main.py` para obter mais detalhes sobre os tipos de entrada suportados.

## Saída

O resultado do processamento será salvo em um arquivo de imagem JPEG nomeado `result_image.jpg` ou em um arquivo de vídeo MP4 nomeado `result.mp4`, dependendo do tipo de entrada.

## Problemas Comuns

Se você encontrar problemas ao executar o script, verifique se todas as dependências estão instaladas corretamente. Além disso, certifique-se de fornecer a entrada correta e válida de acordo com os tipos suportados.

## Créditos

- Este script foi desenvolvido com base nos modelos YOLO do Ultralytics e nas bibliotecas de visão computacional OpenCV e PIL.
- Obrigado à equipe da OpenAI pelo desenvolvimento do modelo de linguagem GPT-3.5 usado para gerar este README.
