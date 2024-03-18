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
  Antes de mais nada, quando refere-se a análise assintótica destas funções MinMax, tem-se essa tabela que reune o "gasto computacional" previsto em funções dos algoritmos representados, demonstrando no melhor caso, pior caso e no caso médio.
  <p align="center">
  <img src="figuras/TABELAMINMAX.png" alt="MINMAXTABELA">
  </p>
Assim sendo tem-se o sistema abaixo contendo os arquivos citados acima além do objetivo de cada função:

- ```vector<int> GerarVetor(int n)```: função responsável por gerar o vetor com o tamanho selecionado e com números aleatórios entre 0 e 1000, retornando o mesmo;
- ```void organizarCrescente(vector<int> vec)```: função responsável por organizar o vetor crescentemente;
- ```void organizarDecrescente(vector<int> vec)```: função responsável por organizar o vetor decrescentemente;
- ```void printarVetor(const vector<int> vec)```: função responsável por imprimir o vetor no terminal;
- ```void registrarVetor(const vector<int> vec, const string nomeArquivo)```: função responsável por escrever no arquivo "vetores.mps" os tempos de execução médio de cada MinMax;
- ```double MinMax1(const vector<int> vec)```: função responsável por verificar o mínimo e máximo do vetor segundo o tipo um estabelecido;
- ```double MinMax2(const vector<int> vec)```: função responsável por verificar o mínimo e máximo do vetor segundo o tipo dois estabelecido;
- ```double MinMax3(const vector<int> vec)```: função responsável por verificar o mínimo e máximo do vetor segundo o tipo três estabelecido;
- ```double Media(const vector<int> vec,int opcao)```: função responsável por fazer a média de dez execuções do MinMax desejado;
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
  Primordialmente utilizei da biblioteca cstdlib devido a função "rand" para gerar os valores aleatórios que serão colocados dentro do vetor através da função "GerarVetor" sendo delimitado entre os inteiros 0 e 1000.
  <br>Após isso, criei as funções "organizarCrescente" e "organizarDecrescente" que utilizam da biblioteca algorithm e functional para assim como foi dito na função organizar o vetor crescentemente e decrescentemente, através da função "sort" e "greater"
  <br>A biblioteca ctime foi utilizada para quantificar o tempo de execução através da função "clock". A biblioteca fstream foi utilizada para acessar o arquivo com "ofstream",e por fim, a biblioteca vector foi utilizada para facilitar a manipulação de vetores.



</p>


## Conclusão
<p align="justify">
</p>

## Referências
DA SILVA, Michel Pires. Material de aula: Análise Assintótica. 8 atrás. 2024. Apresentação de slides. Disponível em: <https://ava.cefetmg.br/pluginfile.php/250215/mod_resource/content/8/Aula1.pdf>. Acesso em 18 mar. 2024.


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
