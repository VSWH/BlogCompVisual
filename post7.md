# Redimensionamento de Imagens Digitais
**21/10/2026**


## Introdução

O redimensionamento de imagens é uma operação comum no processamento digital de imagens. Ele permite alterar as dimensões de uma imagem, seja para aumentar seu tamanho ou para reduzi-lo.

Esse processo está relacionado à amostragem, pois modifica a quantidade de pixels utilizada para representar a imagem. Dependendo de como o redimensionamento é realizado, podem ocorrer perda de detalhes e distorções visuais.

## O que é Redimensionamento de Imagens?

O redimensionamento consiste em modificar a quantidade de pixels de uma imagem para obter novas dimensões.

Existem duas operações principais:

- **Ampliação:** aumenta as dimensões da imagem, sendo necessário estimar os valores dos novos pixels.
- **Redução:** diminui as dimensões da imagem, podendo eliminar informações presentes na imagem original.

Essas operações precisam ser realizadas de maneira adequada para preservar, tanto quanto possível, as características da imagem.

## Ampliação de Imagens

Na ampliação, a imagem passa a ter mais pixels do que originalmente. Como esses novos pixels não existiam na imagem original, seus valores precisam ser determinados por algum método de interpolação.

Uma forma simples de realizar esse processo é o método do **vizinho mais próximo**, que utiliza o valor de um pixel existente para preencher as novas posições.

Embora seja um método simples, a ampliação pode deixar a imagem com aparência pixelizada, principalmente quando o aumento é muito grande.

## Redução de Imagens

Na redução, a quantidade de pixels da imagem diminui. Com isso, algumas informações podem ser perdidas.

De acordo com o conteúdo estudado em aula, uma redução pela metade utilizando o método do vizinho mais próximo pode excluir linhas e colunas alternadas de pixels.

Esse procedimento pode provocar alterações na aparência da imagem, especialmente quando ela apresenta muitos detalhes ou padrões pequenos.

Por isso, é importante considerar como a amostragem será realizada durante a redução.

## Relação com a Amostragem

A amostragem é o processo de representar uma função contínua por meio de valores obtidos em intervalos determinados.

No processamento digital de imagens, ela está relacionada à representação da imagem por pixels.

Durante o redimensionamento, a quantidade de amostras é modificada. Na ampliação, são necessárias novas estimativas de pixels; na redução, parte das amostras deixa de ser utilizada.

Quando a amostragem é insuficiente para representar os detalhes da imagem, podem surgir distorções conhecidas como **aliasing**.

## Como Reduzir as Distorções?

Uma maneira de diminuir os efeitos do aliasing durante a redução de imagens é aplicar um filtro passa-baixa antes da nova amostragem.

Esse filtro suaviza a imagem e atenua as componentes de alta frequência, ajudando a evitar que determinados detalhes sejam representados de maneira incorreta após a redução.

Esse procedimento é especialmente importante quando a imagem contém muitos detalhes ou padrões repetitivos.

## Conclusão

O redimensionamento de imagens digitais é uma operação importante no processamento de imagens e envolve a alteração da quantidade de pixels utilizados na representação.

A ampliação exige a estimativa de novos pixels, enquanto a redução pode eliminar informações da imagem original. Por isso, a escolha do método de redimensionamento influencia o resultado visual.

Além disso, compreender a relação entre redimensionamento, amostragem e aliasing ajuda a entender como preservar a qualidade das imagens durante esse processo.

## Referências

- GONZALES, R. C.; WOODS, R. C. *Processamento Digital de Imagens*. 3. ed. Pearson Prentice Hall, 2010.
- MAJUDER, A.; GOPI, M. *Introduction to Visual Computing: Core Concepts in Computer Vision, Graphics, and Image Processing*. CRC Press, 2018.
- Material de aula: *Domínio da Frequência*. Computação Visual, Prof. André Kishimoto, 2026.


---

[Voltar à página inicial](index.md)
