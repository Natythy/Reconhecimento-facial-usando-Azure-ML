# Reconhecimento Facial Usando Azure ML

![Static Badge](https://img.shields.io/badge/Status_Projeto:-Concluído_(24/Mar/2024)-green)

## Descrição do Projeto

Este desafio é o 3º do Bootcamp [Microsoft Azure AI Fundamentals](https://web.dio.me/track/microsoft-azure-ai-fundamentals). Ele tem como objetivo aprender a usar e testar as seguintes funcionalidades:

- Função 1: Reconhecimento facial em imagens

- Função 2: Extração de textos em imagens

- Função 3: Descrição de imagens

## Acesso

O processo de acesso e criação de recursos para a exploação dos recursos já citados foram feitos com base nas orientações disponíveis pela Microsoft nos seguintes sites (as instruções estão em inglês):

[Reconhecimento facial em imagens](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/04-face.html)

[Extração de textos em imagens](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html)

[Descrição de imagens](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html)

## Insights

### Função 1: Reconhecimento facial em imagens

- Na primeira foto todas as pessoas foram identificadas sem muito problemas.

![Captura de tela 2024-03-23 153231](https://github.com/Natythy/Reconhecimento-facial-usando-Azure-ML/assets/88320974/a9d007f2-cd01-43d4-b0cb-70879aa71674)

- Já na segunda foto, há um homem que tem o rosto à mostra, mas com um braço tampando. A resposta mostra informa o uso de máscara, mostrando que só o fato de ter algo cobrindo o rosto é o suficiente  indicado o uso de máscara, mostrando que qualquer rosto com algo o cobrindo tem na sua descição uso de máscara. Mas como o parte do nariz está exposto, a resposta é que essa "máscara" não cobre o nariz e a boca (mesmo a boca estando tapada).
![Captura de tela 2024-03-23 153131](https://github.com/Natythy/Reconhecimento-facial-usando-Azure-ML/assets/88320974/28c0955f-5cc0-41af-863f-6df80bbd0dcb)

- Esse insight é reforçado no último exemplo. Onde, um braço cobre parte do rosto (no caso os olhos), o que resulta no retorno do uso da "máscara". Mas como nem o nariz e a boca estão cobertos. O retorno é negativo para a "máscara" cobrindo estas partes.
![Captura de tela 2024-03-24 111149](https://github.com/Natythy/Reconhecimento-facial-usando-Azure-ML/assets/88320974/7c9e71ff-c6a3-46dd-87f2-d1d09cf45f90)

### Função 2: Extração de textos em imagens

- Foi feita a detecção dos caractéres sem nenhum problema, independente da cor e do fundo
![Captura de tela 2024-03-24 112834](https://github.com/Natythy/Reconhecimento-facial-usando-Azure-ML/assets/88320974/1dcb12a0-c854-487b-9424-0ed3c8b6db59)

- O mesmo serve para esta imagem apesar de ser em outro sistema de escrita, os caractéres foram identificados (outros caracteres do canto direito da imagem estão mais borradas, dificultando a identificação).
![Captura de tela 2024-03-24 113116](https://github.com/Natythy/Reconhecimento-facial-usando-Azure-ML/assets/88320974/8691e67a-8b77-43ca-a040-b6950b0dce2a)

### Função 3: Descrição de imagens

- A ferramenta deu uma descrição correta, mas muito simples. Não mostrou os detalhes da imagem, como qual é o sabor do suco ou os elementos que compõe a figura.
![Captura de tela 2024-03-24 114729](https://github.com/Natythy/Reconhecimento-facial-usando-Azure-ML/assets/88320974/12ad7773-e829-43a6-a53e-6ce4d638ada4)

- Ao colocar a imagem de um ser humano, a ferramenta foi capaz de trazer mais detalhes, como a cor do cabelo e o posição do braço.
![Captura de tela 2024-03-24 150931](https://github.com/Natythy/Reconhecimento-facial-usando-Azure-ML/assets/88320974/f91d3cd0-6ebb-4cc5-b86f-dd3e5e4d8aa2)

- Na terceira imagem, não foi capaz de identificar a existência de ilustrações ou compreender que era uma propaganda. É possivel perceber que ele realiza uma descrição bem simplificada.
![Captura de tela 2024-03-24 151112](https://github.com/Natythy/Reconhecimento-facial-usando-Azure-ML/assets/88320974/60ffc011-2531-4485-a5e0-04f195779846)

## Conclusões

As ferramentas são efetivas no que prometem, apenas a descrição de imagens que acabou não dando descrições mais detalhadas sobre algumas imagens. Apesar disso são ferramentas que otimizam o tempo de muitas pessoas que precisam extrair texto de imagens ou criar descrições simplificadas para suas imagens. Vale muito apena testar e sendo o caso incoporar na sua rotina.

## Limpando o ambiente

> [!WARNING]
> Após a conclusão do projeto, se não for reaproveitar os recursos utilizados, é aconselhável excluí-los, bem como os grupos de recursos, para que não haja cobranças indevidas na sua Azure Subscription.
