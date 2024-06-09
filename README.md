# Problema de roteamento de veículos (VPR)
- Autores do projeto: Anelise Gonçalves Silva, Gustavo Uchoa Barros e Matheus Zaia Monteiro

### Descrição
- Esse é um trabalho da disciplina de Redes Neurais e Algoritmos Genéticos que tem como objetivo propor um algoritmo genético que busque a melhor solução para o Problema de Roteamento de Veículos (VRP). 

# Introdução Teórica
O Problema de Roteamento de Veículos (VRP) é um problema de otimização combinatória que tem como objetivo encontrar as rotas mais eficientes para uma frota de veículos que precisa fazer entregas ou prestar serviços a um grupo de clientes. O principal objetivo é minimizar o custo total, que pode ser medido em termos de distância percorrida, tempo gasto, entre outros. O VRP pode ser pensado como vários problemas do caixeiro viajante (TSP) combinados. Esse problema é muito comum na vida real, estando presente desde logística de entregas à serviços públicos. Buscar a melhor solução para esse problema e suas variantes vem despertando grande interesse, uma vez que os VRPs desempenham um papel crucial na sociedade moderna, impactando uma ampla gama de setores e contribuindo para operações mais eficientes, econômicas e ambientalmente sustentáveis. No nosso trabalho, exploramos apenas a minimização da distância total percorrida pelos veículos, não incluindo o tempo do percurso, por exemplo. 

Para atacar o problema VRP, utilizamos um algoritmo genético (GA). Algoritmos genéticos são algoritmos estocásticos inspirados na área evolutiva da Biologia, com o objetivo de aproximarem soluções de problemas de otimização. Os GAs iniciam com uma população de respostas aleatórias, e através de operados genéticos como seleção, mutação e cruzamento, selecionam as soluções que apresentam melhor fitness, que é um certo valor dado pela função que está sendo otimizada. 

# Como me orientar no código? 
- O notebook [ga_trab_final.ipynb](https://github.com/lisbylis/Trabalho_Final_Algoritmos_NR/blob/main/ga_trab_final.ipynb) apresenta o algoritmo genético aplicado ao problema VRP.
- As funções e operadores genéticos utilizados no notebook estão presentes no arquivo [ga_vehicle_routing.py](https://github.com/lisbylis/Trabalho_Final_Algoritmos_NR/blob/main/ga_vehicle_routing.py).

# Operadores Genéticos utilizados
- Mutação de Troca: Esse operador funciona trocando a posição de dois elementos em uma sequência. Nesse trabalho, ele funcionou trocando cidades de uma mesma rota.
- Mutação de Partição:  Essa mutação altera a maneira como os elementos são divididos em subgrupos, criando novas partições que podem explorar diferentes configurações do espaço de soluções. Nesse caso, cada indivíduo pode ser reparticionado, alterando as cidades que cada veículo irá visitar.
- Cruzamento Ordenado: Este operador é projetado para trabalhar com representações onde a ordem dos elementos é crucial.
- Seleção por torneio: Esse operador vai selecionar os indíviduos com base no maior fitness!

## Referências 
[1]. https://en.wikipedia.org/wiki/Vehicle_routing_problem 

[2]. https://pt.wikipedia.org/wiki/Algoritmo_gen%C3%A9tico
