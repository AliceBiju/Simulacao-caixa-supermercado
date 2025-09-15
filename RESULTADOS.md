Atividade Programação paralela e distribuída: 

1. Execute a simulação para µ = 5,0, σ = 0,5, N = 100 clientes e 1000 rodadas. Registre a média e o desvio-padrão obtidos.  

2. Varie o número de caixas de 1 para 2 e 3. Compare os resultados obtidos e discuta qualitativamente como mais caixas podem reduzir o tempo médio de atendimento.  

3. Varie σ (ex.: 0,25, 1,0, 2,0) e observe como a variabilidade impacta os resultados médios.  

4. Escreva um parágrafo explicando por que este simulador é considerado estocástico e como isso representa situações reais. 

 

Respostas: 

 

1. 	Média: ~ 5,00 min 

    Desvio Padrão: ~ 0,05 min 

 

2. O tempo médio de atendimento por cliente não muda e abrir mais caixas não faz cada cliente ser atendido mais rápido, mas reduz filas e o tempo de espera total dos clientes, porque o que muda é a variabilidade do sistema, ou seja, com mais caixas os clientes são atendidos em paralelo e o tempo médio do sistema se torna mais estável. 

Caixas   Média     Desvio Padrão    <br>
1        ~5,0      ~0,05            <br>
2        ~5,0      ~0,03            <br>
3        ~5,0      ~0,02            <br>


3.  A média permanece próxima de 5 independente da mudança, mas o aumento dele, faz com que os desvios padrões fiquem mais dispersos e causa maior incerteza nos resultados. 

σ      Média     DP       <br>
0,25   ~5,0      ~0,025   <br>
0,50   ~5,0      ~0,050   <br>
1,00   ~5,0      ~0,100   <br>
2,00   ~5,0      ~0,200   <br>



4. É estocástico porque os tempos de atendimento dos clientes não são fixos, mas sim sorteados a partir de uma distribuição normal, o que dá aleatoriedade nos resultados. Mesmo com os mesmos parâmetros, cada execução pode gerar resultados ligeiramente diferente 

