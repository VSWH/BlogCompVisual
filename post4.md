# Análise e Equalização de Histogramas em Processamento Digital de Imagens
**18/08/2026**


O estudo do **Processamento Digital de Imagens (PDI)** fundamenta-se, em grande parte, na manipulação estatística dos pixels que compõem uma matriz visual. Com base nas diretrizes clássicas da literatura da área (GONZALES; WOODS, 2010), a análise de histogramas constitui uma ferramenta indispensável para o realce visual, a extração de métricas estatísticas e o suporte a processos de segmentação e compressão.

---

## 1. Fundamentos do Histograma Digital

O histograma de uma imagem digital define-se como uma função discreta que relaciona cada nível de intensidade de cinza, representado no intervalo $[0, L - 1]$, à quantidade correspondente de pixels que possuem tal intensidade. A função básica é expressa por:

$$h(r_k) = n_k$$

Onde:
* $r_k$: $k$-ésimo valor de intensidade.
* $n_k$: número de pixels da imagem com intensidade $r_k$.

### Normalização do Histograma

Para fins de modelagem estatística, procede-se frequentemente à normalização do histograma, dividindo-se cada componente $n_k$ pelo número total de pixels da imagem ($M \\times N$). Obtém-se, assim, a estimativa da probabilidade de ocorrência do nível de intensidade:

$$p(r_k) = \\frac{n_k}{M \\times N}$$

> **Nota:** A soma de todos os componentes de um histograma normalizado é unitária, permitindo inferir propriedades visuais fundamentais, tais como características de imagens escuras, claras, de baixo contraste ou de alto contraste.

---

## 2. Equalização e Transformação de Intensidade

O processo de equalização de histograma visa redistribuir os níveis de intensidade por meio da Função de Distribuição Acumulada (CDF), gerando uma imagem de saída com distribuição uniforme e, consequentemente, melhor aproveitamento dinâmico do contraste. 

A forma discreta da transformação $T(r_k)$ é calculada pela expressão:

$$S_k = T(r_k) = (L - 1) \\sum_{j=0}^{k} p_r(r_j) = \\frac{L - 1}{M \\times N} \\sum_{j=0}^{k} n_j$$

Por meio dessa abordagem matemática, valores de intensidade agrupados são expandidos ao longo de toda a faixa disponível, maximizando a nitidez visual da matriz resultante.

---

## 3. Referências Audiovisuais Recomendadas

Para aprofundamento técnico e visualização prática dos conceitos teóricos de histogramas e transformações lineares, recomenda-se o seguinte material de apoio:

1. **"Image Histograms and Equalization Explained" — Computerphile**  
   *Relevância:* Apresenta uma explanação conceitual robusta e didática sobre a dinâmica dos pixels e o comportamento prático de histogramas em ambientes computacionais.
2. **Videoaulas acadêmicas sobre Equalização de Histograma em PDI**  
   *Relevância:* Detalham a resolução passo a passo de exercícios práticos, incluindo a aplicação de matrizes hipotéticas e o cálculo de somatórias acumuladas conforme a formulação de Gonzales e Woods.




---

[Voltar à página inicial](index.md)
