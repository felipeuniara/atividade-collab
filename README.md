# Aula prática: Agendamento de Processos

**Aluno:** Felipe Sperli Neto

Resolução do exercício da disciplina de IA sobre algoritmos de escalonamento de processos.
Notebook original: https://github.com/aannddrree/disciplinaIA/blob/main/aula_pratica_agendamento_processos.ipynb

## Arquivo

- `aula_pratica_agendamento_processos_resolvido.ipynb`: notebook com as células da aula e a resolução do desafio (seção 8), já executado.

## O que foi feito

1. Adicionei o processo P4 (chegada 3, burst 1).
2. Comparei FCFS com Round Robin usando quantum 1, 2 e 4.
3. Respondi qual política favoreceu o P4.
4. Implementei o SJF (não preemptivo).
5. Montei uma tabela e um gráfico comparando as políticas e escrevi a conclusão.

## Resultados

| Política | Espera média (ms) | Espera do P4 (ms) | Fatias de CPU |
|---|---|---|---|
| FCFS | 5,00 | 9 | 4 |
| RR q=1 | 4,25 | 2 | 13 |
| RR q=2 | 4,50 | 5 | 7 |
| RR q=4 | 5,25 | 7 | 5 |
| SJF | 4,00 | 3 | 4 |

O P4 foi mais favorecido pelo Round Robin com quantum 1, seguido pelo SJF. O SJF teve a menor espera média.

## Como abrir

No Google Colab: **Arquivo → Fazer upload de notebook** e escolher o `.ipynb`.
Para rodar localmente é preciso Python 3 com `matplotlib` e Jupyter.
