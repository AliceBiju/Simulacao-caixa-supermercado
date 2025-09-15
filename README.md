# Simulação de Atendimento em Caixas de Supermercado

Este repositório contém a implementação de um simulador estocástico em Java para analisar o atendimento em caixas de supermercado. O objetivo é estimar a média e o desvio-padrão do tempo de atendimento de clientes e estudar o impacto de diferentes parâmetros, como número de caixas e variabilidade do atendimento.

## Tecnologias usadas

* Java
* Git/GitHub

## Como executar

1. Compile os arquivos Java:

```bash
javac src/*.java
```

2. Execute o programa:

```bash
java -cp src Main
```

## Resultados das Simulações

### Variação de σ

```
σ      Média     DP
0,25   ~5,0      ~0,025
0,50   ~5,0      ~0,050
1,00   ~5,0      ~0,100
2,00   ~5,0      ~0,200
```

*Observação:* A média permanece próxima de 5,0. À medida que σ aumenta, a variabilidade individual cresce, aumentando a incerteza nos resultados médios.

### Variação do número de caixas

```
Caixas   Média     Desvio Padrão
1        ~5,0      ~0,05
2        ~5,0      ~0,03
3        ~5,0      ~0,02
```

*Observação:* A média por cliente não muda significativamente, mas mais caixas reduzem a variabilidade do tempo médio do sistema, tornando os resultados mais estáveis.

## Por que o simulador é estocástico

O simulador é considerado estocástico porque os tempos de atendimento são gerados aleatoriamente a partir de uma distribuição normal. Mesmo com os mesmos parâmetros, cada execução gera resultados diferentes, refletindo a variabilidade real de atendimentos em supermercados, como quantidade de itens, forma de pagamento e imprevistos no caixa.

## Estrutura do repositório

```
simulacao-caixa-supermercado/
├─ src/
│  ├─ SimulacaoCaixaSupermercado.java
│  └─ Main.java
├─ RESULTADOS.md
└─ README.md
```

## Autor

* Alice Santos Monteiro de Barros
