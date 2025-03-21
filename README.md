# Mapa Logístico - Análise e Visualização

Este projeto explora o mapa logístico, um sistema dinâmico que exibe comportamento caótico. O código em Python utiliza bibliotecas como `matplotlib`, `numpy`, `scipy` e `numba` para gerar e visualizar as iterações do mapa logístico.

## Bibliotecas Utilizadas

* `matplotlib.pyplot`: Para criação de gráficos e visualizações.
* `numpy`: Para operações numéricas eficientes e manipulação de arrays. 
* `math`: Para funções matemáticas. 
* `random`: Para geração de números aleatórios. 
* `scipy`: Biblioteca científica para computação numérica, com `scipy.special` para funções matemáticas especiais e `scipy.optimize` para ajuste de curvas. 
* `numba`: Compilador JIT (`Just-In-Time`) para otimizar o desempenho do código, incluindo paralelização com `numba.njit` e `numba.prange`.
* `time`: Para medir o tempo de execução de diferentes partes do código. 

## Geração do Mapa Logístico

O código implementa a função logística iterativamente para diferentes valores do parâmetro μ. A função logística é definida como:

$$x_{1}=\mu x_{0}(1-x_{0})$$

Onde:

* `x0` é o valor inicial.
* `mu` é o parâmetro que controla o comportamento do sistema.
* `x1` é o próximo valor na iteração. 

## Visualização dos Resultados

O projeto gera diferentes visualizações para analisar o comportamento do mapa logístico:

1.  **Diagrama de Bifurcação:** Este diagrama plota os valores de `x` em função de `mu`, mostrando como o comportamento do sistema se bifurca e se torna caótico à medida que `mu` aumenta. 

2.  **Histogramas:** Histogramas são gerados para diferentes valores de `mu` para visualizar a distribuição dos valores de `x`. 

3.  **Diagramas de Iteração:** Estes diagramas mostram as iterações do mapa logístico para valores específicos de `mu`, traçando a evolução de `x` ao longo das iterações, juntamente com a função logística e a linha de identidade.

## Código

O código é estruturado em blocos que realizam as seguintes operações:

* **Importação de bibliotecas:** As bibliotecas necessárias são importadas no início do script. 
* **Geração de dados:** Os valores de `mu` e os valores iniciais de `x` são definidos, e as iterações do mapa logístico são calculadas. 
* **Visualização:** Os dados gerados são plotados utilizando `matplotlib.pyplot` para criar os diagramas de bifurcação, histogramas e diagramas de iteração. 

Este README fornece uma visão geral do projeto e do código utilizado para explorar o mapa logístico.
