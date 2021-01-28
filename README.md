# GraphProcessing
Trabalho da Disicplina Grafos e Algoritmos Computacionais

## Objetivo

Implementar uma biblioteca em Python capaz de processar dados na forma de grafos não direcionados. A biblioteca deve representar o grafo internamente como uma Lista de Adjacência, ser capaz de ler os dados de um grafo a partir de um arquivo texto e oferecer um conjunto de funções capaz de processar o grafo e extrair informações. Para testar a biblioteca, a mesma será submetida ao processamento de um caso de uso descrito neste documento.

## Funções Básicas da biblioteca: 

* Graph               - criar um novo grafo vazio.
* loadData            - carregar um grafo a partir de um dado arquivo de dados em formato texto. O caminho ao arquivo é passado como parâmetro da função. A primeira linha do arquivo possui o número de vértices do grafo e as demais linhas possui os identificadores de dois vértices adjacentes separados por um espaço em branco.
* minDegree           - devolve o grau mínimo entre todos os vértices do grafo.
* maxDegree           - devolve o grau máximo entre todos os vérices do grafo.
* numEdges            - devolve o número de arestas do grafo.
* numVertex           - devolve o número de vértices do grafo. 
* components          - devolve o número de componentes conexos do grafo. Essa função deve ser implementada através de uma busca em profundidade no grafo.

## Caso de Uso da Biblioteca

Ler o arquivo de dados "dblp.txt" (que pode ser baixado em https://drive.google.com/file/d/185tfrhy7v0rK8C_kSirjufuf07VFgvvH/view?usp=sharing), e processar o grafo correspondente com a biblioteca implementada. Os dados desse arquivo refletem a rede de colaborações de entre pesquisadores em computação. Cada vértice identifica um pesquisador e cada aresta identifica que já houve colaboração entre os pesquisadores. 

Resultados a serem exibidos como resultado do teste da biblioteca:  

* Número de pesquisadores (vértices)
* Número de colaborações (arestas)
* Id do pesquisador que mais colaborou e quantas foram as colaborações (envolve o grau máximo) 
* Menor colaboração (grau mínimo) 
* Número de subredes de colaboração (número de componentes conexos do grafo)
