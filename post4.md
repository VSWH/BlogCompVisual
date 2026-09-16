# Como Ensinar um PC a Desenhar: Recursos
**18/08/2026**


Na aula de computação visual desta semana, realizamos uma atividade em que contamos a quantidade de animais em uma foto para entender o seguinte conceito: humanos desenham o contorno de um objeto em dois segundos, enquanto computadores se perdem em qualquer textura de grama ou sombra de parede.

Recursos
1. Vídeos do Computerphile (YouTube)
Finding Edges (Sobel Operator): Mike Pound desenha em papel milimetrado como matrizes 3x3 transformam fotos em mapas de relevo.

Canny Edge Detector: Explica a técnica de histerese como um jogo de dominó visual para não quebrar linhas.


2. Galeria Interativa do scikit-image
O exemplo plot_canny da documentação oficial permite alternar o valor de sigma (suavização gaussiana) em tempo real.

Mostra na prática como um sigma baixo detecta até poros da pele, enquanto um valor alto preserva apenas a silhueta principal.


3. Topografia 3D de Pixels (ImageJ / Matplotlib)
Ferramentas que tratam intensidade de luz como altitude (branco = pico, preto = vale).

Deixa claro por que ruído quebra derivadas: fotos ruidosas viram "campos de brita pontiaguda", impossibilitando achar o contorno real sem suavização prévia.


Conclusões
Detectar contornos não é achar uma verdade absoluta na imagem, mas sim decidir quanto ruído você aceita ignorar para extrair a forma do mundo real.


---

[Voltar à página inicial](index.md)
