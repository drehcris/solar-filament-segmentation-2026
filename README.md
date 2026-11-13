# Solar Filament Segmentation 2026

Solução baseada em U-Net treinada com GPU no Kaggle para segmentação de filamentos solares.

## Arquivos

- `unet_gpu_kaggle.ipynb`: notebook de treinamento e inferência.
- `unet_best.pt`: melhor modelo treinado.
- `submission_unet.csv`: arquivo enviado ao Kaggle.
- `requirements.txt`: dependências do projeto.

## Método

As imagens são convertidas para grayscale e redimensionadas para 512×512. A U-Net é treinada com BCE Loss + Dice Loss. 
Depois, as máscaras são redimensionadas para 2048×2048, separadas em componentes conectados e convertidas para RLE COCO.

## Resultado

- Melhor Dice de validação: `PREENCHER`
- Score público no Kaggle: `PREENCHER`
- GPU utilizada: `PREENCHER`

## Reprodução

1. Abrir o notebook no Kaggle.
2. Adicionar os dados da competição.
3. Ativar GPU.
4. Executar todas as células.
5. Enviar `submission_unet.csv` no Kaggle.
