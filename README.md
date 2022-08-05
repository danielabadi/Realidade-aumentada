# Trapalho Prático 2: Realidade Aumentada
## Objetivo

O objetivo deste trabalho é detectar e localizar alvos nos quadros (frames) de um vídeo e inserir na cena objetos tridimensionais acima de cada alvo detectado. Para este trabalho, o objeto tridimensional será um cubo tridimensional e um modelo 3D (o Pikachu). A figura abaixo mostra um exemplo de como um frame do vídeo final deve ficar após o processamento.

![image](https://user-images.githubusercontent.com/48056794/183140526-4509856d-a0df-43ef-81bc-8f7d9202fa44.png)

## O que deve ser feito

O trabalho deverá ser implementado em um Notebook Python e as decisões de implementação deverão ser documentadas no próprio Notebook. Siga os passos abaixo na sua implementação:
1. O primeiro passo será a calibração da câmera utilizando o vídeo com o tabuleiro de xadrez como alvo de calibração. Nesta etapa será realizada a estimação dos parâmetros intrínsecos da câmera. 
2. Depois de estimada a matriz de parâmetros intrínsecos, o aluno deverá implementar um método de detecção e localização da posição e orientação do alvo em cada frame do vídeo. Pode-se utilizar funções da OpenCV para ler vídeos, imagens, calcular a matriz de homografia, recortar e colar, binarizar, detectar bordas, detectar quinas e detecar poligonos.
3. Neste passo você deverá codificar uma função para obter a pose da câmera (parâmetros extrínsecos).
4. Finalmente um cubo (objeto tridimensional) deverá ser incluído na cena na posição o orientado de cada alvo detectado (a orientação do cubo deve ser mostrada). A renderização deverá ser feita utilizando somente as funções da OpenGL (o aluno não deve usar funções da OpenCV para renderizar objetos na cena).
5. O modelo do Pikachu deverá ser animado sendo rotacionado em cada frame em torno do eixo Z. Note que o cubo não deve ser rotacionado, apenas o modelo do Pikachu.

Mais detalhes no arquivo de especificação.
