# Projeto: 🎨 Recuperação de Obras de Arte

## Desenvolvido por: Fernanda Paula Rocha

### Introdução 🌟

Desvende o universo das artes visuais com o projeto de Recuperação de Obras de Arte! Utilizando técnicas avançadas de processamento de imagem, exploramos características de cor e textura para identificar obras semelhantes. Parte deste projeto ganhou vida durante a disciplina "Técnicas Avançadas para Captura e Tratamento de Dados" no MBA de Ciência de Dados da USP São Carlos.

### Técnicas Utilizadas 🖌️

1. **Local Binary Pattern (LBP):** Extrai características de textura comparando a intensidade de um pixel com seus vizinhos.
   
2. **VGG16:** Uma poderosa rede neural convolucional treinada no conjunto de dados ImageNet, capaz de extrair características visuais complexas.

### Conjunto de Dados 📸

O diretório "paintings22" abriga uma coleção diversificada de imagens representando obras de arte. A busca por similaridade é realizada em relação à imagem de consulta "query.jpg", desafiando o sistema a identificar obras semelhantes em estilos e autores diversos.

### Objetivo 🚀

Desenvolver um sistema robusto de recuperação de imagens que, usando LBP e VGG16, encontre obras de arte semelhantes à imagem de consulta. Avaliaremos quão eficaz cada modelo é na tarefa, proporcionando uma compreensão profunda da capacidade de extração de características de cada técnica.

### Mais Informações 🔍

Dada a imagem "query.jpg", a busca por similaridade incorpora informações de cor e textura. A composição inclui:

- **Cor:** Conversão para um canal único e criação de um histograma normalizado.
  
- **Textura:** Utilização de Local Binary Pattern (LBP) com raio 1.45 e 16 pontos, gerando 18 características.

Os vetores resultantes desses processos são combinados para formar um descritor que incorpora informações de cor e textura. Esse descritor é utilizado para buscar as 5 imagens mais similares no diretório "paintings22", considerando a distância L1 na comparação.

O resultado da busca é apresentado, exibindo a imagem de consulta e as 5 imagens recuperadas, com nomes e valores das distâncias L1. Este processo busca identificar obras visualmente similares, mesmo quando o autor é desconhecido.

Aventure-se no mundo da arte e da tecnologia, explorando as nuances visuais que conectam obras de diferentes épocas e estilos! 🎨💡
