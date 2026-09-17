# Atividade Prática — Programação Assistida por Inteligência Artificial

**Disciplina:** Programação Assistida por Inteligência Artificial
**Professora:** Kadidja Valéria
**Projeto escolhido:** Calculadora Simples (Nível Básico)

## Objetivo

Utilizar IA como apoio contínuo à programação, indo além do código básico
para explorar refatoração inteligente, seguindo o Ciclo de Colaboração
Humano-IA:

1. **Contextualizar & Sugerir (IA)** — a IA analisa o pedido e o código
existente e gera uma sugestão inicial.
2. **Avaliar Criticamente (Humano)** — o humano revisa a lógica, a
segurança e a aderência ao problema.
3. **Refatorar & Ajustar (Humano + IA)** — o código é otimizado através
de prompts iterativos.
4. **Decidir & Integrar (Humano)** — o humano assume a responsabilidade
final pelo código.

## Arquivos do projeto

- `calculadora_base.py` — versão inicial, sugerida diretamente pela IA.
- `calculadora_refatorada.py` — versão final, após avaliação crítica e
refatoração.

## Etapa 1 — Avaliação crítica da versão base

A versão base (`calculadora_base.py`) resolve o problema, mas apresenta
falhas que só aparecem sob revisão humana atenta:

| Problema | Risco |
|---|---|
| Sem tratamento de divisão por zero | O programa quebra com `ZeroDivisionError` |
| Sem tratamento de entrada inválida | O programa quebra com `ValueError` se o usuário digitar texto |
| Operações soltas em `if`s | Código pouco reutilizável e difícil de testar |
| Sem loop de repetição | Usuário precisa reiniciar o programa a cada cálculo |

## Etapa 2 — Refatoração sugerida

Prompt estruturado usado (seguindo o modelo "Roteiro de Prompts" da aula):

> "Refatore esta calculadora separando cada operação em uma função,
> trate divisão por zero e entrada inválida, e permita repetir o
> cálculo sem reiniciar o programa."

Mudanças aplicadas na versão refatorada:

- Cada operação (`somar`, `subtrair`, `multiplicar`, `dividir`) virou
uma função pura e testável.
- Um dicionário (`OPERACOES`) substitui a cadeia de `if/elif` —
padrão mais "pythônico" e fácil de estender.
- `try/except` trata `ValueError` (entrada não numérica) e
`ZeroDivisionError` (divisão por zero) sem derrubar o programa.
- Um `while True` com confirmação (`s/n`) permite repetir o cálculo.

## Etapa 3 — Decisão final (responsabilidade humana)

A IA sugeriu a estrutura e o padrão de código, mas as decisões finais
foram humanas:

- Manter o loop de repetição em vez de encerrar após um único cálculo.
- Definir que erros de entrada devem pedir novamente o valor, em vez de
encerrar o programa.
- Validar, por meio de testes manuais, que todas as operações e o caso
de divisão por zero funcionam corretamente antes de considerar o
código pronto.

## Conclusão

Esse exercício ilustra o conceito central da aula: **a IA não substitui
o desenvolvedor, mas amplia sua capacidade criativa e produtiva**. A
máquina entregou velocidade e sintaxe otimizada; o papel humano foi
decidir, validar e dar direção — a "assinatura" no commit final é
sempre humana.
