# Aula 02 – Engenharia de Prompt

## 1. Identificação
- Disciplina: Tendências em Ciências da Computação
- Unidade: I - Fundamentos
- Turma: Ciência da Computação
- Data: 20/08/2026
- Integrantes: Luan Bispo Silva (32635648) - Lucas Vitor Lima Santana (33747644) - João Gabriel Rodrigues Pereira (3604408)

## 2. Problema Escolhido
Estudantes do primeiro semestre do curso de Ciência da Computação encontram dificuldade em estruturar uma rotina de estudos prática e equilibrada para aprender lógica de programação com Python, frequentemente sobrecarregando-se com excesso de teoria e pouca aplicação prática.

## 3. Objetivo
Utilizar a IA generativa como suporte pedagógico para construir um plano de estudos estruturado de 4 semanas, focado em lógica de programação com Python, com carga horária viável e exercícios práticos progressivos.

## 4. Prompt Inicial
Crie um plano de estudos de programação em Python para iniciantes.

## 5. Resultado Inicial
Resposta da IA:
Aqui está um plano de estudos para aprender Python:
- Mês 1: Introdução, variáveis, tipos de dados, operadores e condicionais (if/else).
- Mês 2: Laços de repetição (for, while), listas, dicionários e tuplas.
- Mês 3: Funções, módulos, manipulação de arquivos e tratamento de erros.
- Mês 4: Programação Orientada a Objetos (POO), bibliotecas e projetos finais.
Dica: Pratique todos os dias e leia a documentação oficial.

## 6. Análise Crítica
- O que funcionou: A IA listou os tópicos essenciais em uma ordem conceitual aceitável.
- O que não funcionou: A resposta assumiu uma duração de 4 meses em vez de um plano focado de curto prazo, não estimou carga horária semanal nem sugeriu exercícios aplicados.
- O que faltou: Falta de contexto sobre o nível do estudante, ausência de divisão em horas/semana, formato não estruturado (listagem genérica) e ausência de critérios de progressão.
- O que precisa ser validado: Se o volume de conteúdo é viável para quem nunca programou sem causar sobrecarga cognitiva.

## 7. Prompt Refinado
PAPEL:
Você é um professor universitário e tutor de programação para cursos de Computação.

CONTEXTO:
O público-alvo são estudantes ingressantes no primeiro semestre da graduação em Ciência da Computação que nunca tiveram contato prévio com programação e possuem rotina acadêmica intensa.

OBJETIVO:
Criar um cronograma de estudos focado em Lógica de Programação com Python para 4 semanas de nivelamento.

TAREFA:
Elabore um cronograma semanal detalhando os tópicos conceituais, atividades práticas progressivas e tempo sugerido.

RESTRIÇÕES:
- Limite máximo de 6 horas semanais de estudo.
- Nível estritamente introdutório (variáveis, condicionais, repetição e listas básicas).
- Sem uso de jargões técnicos complexos sem explicação.
- Cada semana deve conter um minidesafio prático aplicável.

FORMATO DE SAÍDA:
Apresente o resultado em uma tabela Markdown contendo exatamente as seguintes colunas:
| Semana | Conceito Central | Atividade Prática / Mini-Projeto | Carga Horária |

Ao final da tabela, liste 3 perguntas de autoavaliação para o estudante testar seu aprendizado.

CRITÉRIOS DE QUALIDADE:
O plano deve ser realista, pedagogicamente progressivo e direto ao ponto.

## 8. Resultado Refinado
| Semana | Conceito Central | Atividade Prática / Mini-Projeto | Carga Horária |
| :--- | :--- | :--- | :--- |
| Semana 1 | Variáveis, Entrada/Saída de Dados e Tipos Básicos (str, int, float) | Criar um programa de console que calcula a média final de um aluno e exibe uma mensagem personalizada. | 6h (2h teoria / 4h prática) |
| Semana 2 | Tomada de Decisão e Estruturas Condicionais (if, elif, else) | Desenvolver um simulador de caixa eletrônico simples (validação de saldo e saque). | 6h (2h teoria / 4h prática) |
| Semana 3 | Laços de Repetição (while e for) | Construir um jogo de adivinhação de números com limite de tentativas e dicas de maior/menor. | 6h (1h teoria / 5h prática) |
| Semana 4 | Coleções Básicas (Listas) e Modularização Simples | Criar um gerenciador de tarefas (To-Do List) no terminal para adicionar, listar e remover itens. | 6h (1h teoria / 5h prática) |

Perguntas de Autoavaliação:
1. Qual a diferença prática entre utilizar uma estrutura if-elif-else e múltiplos blocos if independentes?
2. Em quais situações um laço while é preferível em relação ao laço for?
3. Como as listas facilitam a manipulação de múltiplos dados em comparação com a criação de variáveis individuais?

## 9. Técnicas Utilizadas
- [x] Role Prompting (Papel de tutor acadêmico)
- [ ] Few-Shot Prompting
- [x] Contexto (Estudantes do 1º semestre de Computação)
- [x] Restrições (6h semanais, 4 semanas, sem termos complexos)
- [x] Formato de saída (Tabela Markdown estruturada + perguntas)
- [ ] Prompt em etapas
- [x] Refinamento iterativo

## 10. Comparação
| Critério | Prompt A (Inicial) | Prompt B (Refinado) |
| :--- | :--- | :--- |
| Clareza | Baixa (aberto a interpretações) | Alta (diretrizes explícitas) |
| Contexto | Inexistente | Definido (ingressantes do 1º semestre) |
| Relevância | Genérica e fora da carga horária real | Alta e adaptada ao escopo do estudante |
| Organização | Lista de tópicos sem granularidade | Tabela estruturada por semana e carga horária |
| Precisão | Baixa (misturou tópicos avançados como POO) | Alta (focado apenas em lógica essencial) |
| Utilidade | Baixa para planejamento imediato | Pronta para execução pelo estudante |

## 11. Validação
A resposta foi validada comparando a sequência didática com a ementa de disciplinas introdutórias de algoritmos, confirmando que a carga horária de 6h semanais é coerente com a complexidade dos mini-projetos propostos.

## 12. Ética e Responsabilidade
Riscos identificados: A IA pode sugerir bibliotecas obsoletas, propor exercícios com complexidade incompatível para iniciantes ou gerar dependência excessiva no estudante, que pode deixar de exercitar a resolução autônoma de problemas.

Mitigação: A supervisão humana permanente é indispensável para revisar o código gerado, validar as boas práticas pedagógicas e garantir a veracidade técnica do conteúdo.

## 13. Take Away
Cognitivo: A estruturação de prompts iterativos demonstra que a IA generativa não substitui a reflexão humana; ela atua como um amplificador que depende fundamentalmente do rigor, da clareza e do direcionamento fornecidos pelo operador.

Ético: A responsabilidade sobre o conteúdo gerado, a integridade técnica, eventuais vieses e a validação do conhecimento produzido cabe integralmente ao profissional que opera a ferramenta.
