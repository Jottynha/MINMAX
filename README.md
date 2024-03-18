<h1 align="center" font-size="200em"><b>Avaliação dos Algoritmos Minimax</b></h1>

## Introdução
<p align="justify">
  Este é um programa desenvolvido em C++ para a disciplina de Algoritmos e Estruturas de Dados I. O mesmo tem por objetivo simular algoritmos Minimax através de processos distintos, verificando o tempo de execução dos três algoritmos e analisando a eficiência destes processos. Seguindo as instruções associadas à aula de análise assintótica, que é responsável por observar a capacidade ou computabilidade dos algoritmos, definindo um "custo" para execução destes. Pois atualmente há uma grande exigência do mercado quanto a diminuição dos custos visando o aprimoramento dos algoritmos.
</p>

## Objetivos
<p align="justify">
  Este programa tem por objetivo verificar o tempo de execução (dado em nanosegundos) dos três algoritmos que implementam a busca de valores mínimos e máximos dentro de um vetor de três maneiras distintas, segundo alguns parâmetros sugeridos dentro de aula.
  O sistema em si deverá identificar qual dos três algoritmos está sendo executado, verificar sua eficiência de execução no mesmo vetor com três ordenações distintas (sendo estas aleatória, crescente e decrescente). Além de repetir este processo por dez vezes e criando uma média do mesmo para retorno do resultado.
  Os tamanhos selecionados para este programa quanto aos vetores foram: 1000, 10.000, 100.000 e 500.000. Sendo um vetor de números inteiros que variam de 0 a 1000.
</p>
<p align="justify">
  Verifica-se abaixo as três arquiteturas de códigos (Em Pascal) que devem ser adaptadas para o programa em C++:
  <p align="center">
  <img src="figuras/MINMAX1.png" alt="MINMAX1">
  <img src="figuras/MINMAX2.png" alt="MINMAX2">
  <img src="figuras/MINMAX3.png" alt="MINMAX3">
  </p>
</p>

## Arquivos
### dataset
- ```vetores.mps.txt```: arquivo que contém os tempos de execução do programa;
## src
- ```MinMax.hpp```: arquivo que contém o cabeçalho das funções MinMax;
- ```MinMax.cpp```: arquivo que contém o código de funcionamento das funções MinMax e auxiliares (manipulação);
- ```main.cpp```: arquivo principal.

## Resolução do problema
<p align="justify">
  Antes de mais nada, quando refere-se a análise assintótica destas funções MinMax, tem-se essa tabela que reune o "gasto computacional" em funções dos algoritmos representados, demonstrando no melhor caso, pior caso e no caso médio.
  <p align="center">
  <img src="figuras/TABELAMINMAX.png" alt="MINMAXTABELA">
  </p>

<p align="center">
  <img src="figuras/MINMAXHPP.png" alt="MINMAX.hpp">
  <img src="figuras/MINMAXCPP1.png" alt="MINMAX.cpp">
  <img src="figuras/MINMAXCPP2.png" alt="MINMAX.cpp">
  <img src="figuras/MINMAXCPP3.png" alt="MINMAX.cpp">
  <img src="figuras/MINMAXCPP4.png" alt="MINMAX.cpp">
  <img src="figuras/MINMAXCPP5.png" alt="MINMAX.cpp">
  <img src="figuras/MINMAXCPP6.png" alt="MINMAX.cpp">
  <img src="figuras/MAIN.png" alt="Main">
</p>




</p>


## Conclusão
<p align="justify">
</p>

## Referências



## Compilação e execução
* | Comando                |  Função                                                                                           |                     
  | -----------------------| ------------------------------------------------------------------------------------------------- |
  |  `make clean`          | Apaga a última compilação realizada contida na pasta build                                        |
  |  `make`                | Executa a compilação do programa utilizando o gcc, e o resultado vai para a pasta build           |
  |  `make run`            | Executa o programa da pasta build após a realização da compilação                                 |

## Contato
<div>
<a style="color:black" href="mailto:jprs1308@gmail.com?subject=[GitHub]%20Source%20Dynamic%20Lists">
✉️ <i>jprs1308@gmail.com</i>
</a>
