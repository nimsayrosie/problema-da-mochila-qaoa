# Problema da Mochila com QAOA (Quantum Approximate Optimization Algorithm)

> Trabalho desenvolvido pelo **Grupo 2 Q-Health** no segundo módulo do Brazil Quantum Tech programa realizado pelo CESAR School e pelo Instituto de Pesquisas ELDORADO, em parceria com a SOFTEX e o Ministério da Ciência, Tecnologia e Inovação (MCTI).  .

---

## Integrantes

| Nome |
|------|
| Carlos Eduardo da Silva Almeida |
| Carlos Mello |
| Gabriel Ferreira Masson |
| Hilson Gomes Vilar de Andrade |
| Luiza Marinho Diniz Schirmer |
| Marilio Cavalcanti de Moura |
| Melissa Figueira Fagundes |
| Yasmin Lourdes e Silva |

---

## Descrição do Projeto

Este projeto implementa o **QAOA (Quantum Approximate Optimization Algorithm)** para resolver o clássico **Problema da Mochila (Knapsack Problem)**.

### O Problema da Mochila
Dado um conjunto de itens com pesos e valores, o objetivo é selecionar quais itens incluir em uma mochila de forma a **maximizar o valor total** sem exceder a **capacidade máxima de peso**.

### O Algoritmo QAOA
O QAOA é um algoritmo **híbrido quântico-clássico** que:
1. Codifica o problema como um **Hamiltoniano de custo**
2. Aplica camadas alternadas de operadores quânticos
3. Usa um otimizador clássico para ajustar os parâmetros
4. Encontra soluções aproximadas para problemas de otimização combinatória

---

## Estrutura do Notebook

## Estrutura do Notebook

O projeto está organizado no arquivo `QAOA_ProblemaDaMochila.ipynb` seguindo o fluxo lógico abaixo:

└── QAOA_ProblemaDaMochila.ipynb
    ├── 1. Definição do problema no formato QUBO
    │   └── Conversão do Problema da Mochila para QUBO
    │       ├── h → Coeficientes diagonais (pesos/valores individuais)
    │       └── J → Coeficientes de interação (restrições de capacidade)
    ├── 2. Circuito QAOA
    │   ├── Operador de Custo Uc(γ)
    │   ├── Operador de Mistura Um(β)
    │   └── Otimização de parâmetros via Gradiente Descendente
    ├── 3. Medição e Resultado
    │   └── Análise da distribuição de probabilidades dos estados quânticos
    └── 4. Validação
        └── Comparação da solução quântica com a solução ótima (Brute Force)

