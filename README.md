# SCC0220 - Laboratório de Introdução à Ciência da Computação II

Trabalhos da disciplina **SCC0220 - Laboratório de Introdução à Ciência da Computação II**, que propõe implementar algoritmos variados e comparar sua eficiência.

<p align="center">
  <img alt="Disciplina" src="https://img.shields.io/badge/SCC0220-Laborat%C3%B3rio%20de%20Introdu%C3%A7%C3%A3o%20%C3%A0%20Ci%C3%AAncia%20da%20Computa%C3%A7%C3%A3o%20II-blue?style=for-the-badge">
  <img alt="Instituição" src="https://img.shields.io/badge/USP-Universidade%20de%20S%C3%A3o%20Paulo-orange?style=for-the-badge">
</p>

> **Disciplina:** SCC0220 - Laboratório de Introdução à Ciência da Computação II <br>
> **Instituição:** USP - Universidade de São Paulo

<p align="center">
  <img src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black" alt="C" />
  <img src="https://img.shields.io/badge/Make-6D00CC?style=for-the-badge&logo=gnu&logoColor=white" alt="Make" />
  <img src="https://img.shields.io/badge/Shell-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white" alt="Shell" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy" />
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge" alt="Matplotlib" />
</p>

## Requisitos

- Compilador **C** (por exemplo, `gcc`) e **Make**
- **Bash** para os scripts de automação
- **Python 3** com `numpy` e `matplotlib` para os gráficos de tempo (`TimeTest/grafico.py`)

## Como Executar

Compile os fontes da pasta do trabalho desejado:

```bash
gcc Aula02_Exponenciacao/*.c -o programa
```

Os casos de teste de cada trabalho ficam na pasta correspondente (`casoteste`, `casos_run` etc.).

## Estrutura do Projeto

- `/Aula01_Karatsuba` a `/Aula10_MSC`: um trabalho por pasta, com código e casos de teste.
- `/CodigosBase`: códigos base de apoio.
- `/TimeTest`: medição de tempo: `juiz.py` e `juiza2.sh` (execução dos programas), `grafico.py` (gráficos, com `numpy` e `matplotlib`) e os resultados por aula.

Todos os trabalhos possuem um relatório (`Relatório - Aula N.docx`) detalhando o processo de construção dos códigos e os métodos de avaliação. Várias pastas trazem `Makefile` e scripts de automação (`CasaAutomatica.sh`, entre outros) que rodam os casos e geram os tempos e gráficos.

## Trabalhos

1. **Multiplicação:** multiplicação convencional $O(n^{2})$ e algoritmo de Karatsuba $O(n^{\log_2 3}) \approx O(n^{1.58})$.
2. **Exponenciação:** iterativa $O(n)$ e por divisão e conquista (exponenciação rápida) $O(\log n)$.
3. **Seleção:** ordenação por seleção $O(n^{2})$ (com TAD de pilha) e Shell Sort $O(n^{3/2})$ sobre registros de jogador (`nome nota`), com desempate lexicográfico.
4. **Notáveis:** lê uma planilha `.csv` de notas e imprime os `k` alunos com maior aumento de nota.
5. **Bubble and Quick:** BubbleSort $O(n^{2})$ e QuickSort $O(n \log n)$ para ordenar pratos por tempo e prioridade.
6. **A outra pilha:** MergeSort $O(n \log n)$ e HeapSort $O(n \log n)$ para ordenar pratos por tempo e prioridade.
7. **A outra pilha:** RadixSort $O(n)$ e StoogeSort $O(n^{2.7})$ para ordenar cartas de baralho.
8. **Buscando problemas:** busca binária $O(\log n)$ para achar cartas danificadas, comparada à busca sequencial $O(n)$.
9. **O melhor caminho:** árvore binária de busca $O(\log n)$ comparada a uma busca linear (DFS ou BFS) $O(n)$.
10. **MSC:** Máxima Subsequência Consecutiva, com HashMap e com ordenação.
11. **Tour:** simula um grafo e o percorre por um número de passos.
