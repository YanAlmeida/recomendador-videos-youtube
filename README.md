# recomendador-videos-youtube

O projeto consiste em um recomendador de vídeos similares para o Youtube, que recebe uma URL de vídeo e retorna um vídeo similar, bem como seu resumo.

Na primeira etapa do projeto, extraiu-se uma base com IDs de vídeos do Youtube (temas variados) através da Youtube Data API.
Então, utilizou-se o software Youtube-DL para baixar as legendas em inglês dos vídeos, efetuou-se o pré-processamento e a vetorização (utilizando TF-IDF) dos textos. Para comparação do texto inserido com os textos da base, utilizou-se a métrica de similaridade por cosseno. Para sumarização da legenda do vídeo recomendado, construiu-se uma matriz de similaridade baseada na distância de cosseno entre as sentenças para determinar aquelas que seriam utilizadas.
