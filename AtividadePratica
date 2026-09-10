# Atividade Prática A2 — Suíte de Prompts Iterativos com IA Generativa

**Disciplina:** Fundamentos de AI e Engenharia de Prompt
**Valor:** 0,5 ponto | **Formato:** Em grupo | **Entrega:** Repositório no GitHub

## 1. Tema — Definição do Problema Real

Estudantes universitários frequentemente cursam **várias disciplinas ao mesmo tempo**, cada uma com datas de prova diferentes, níveis de dificuldade diferentes e cargas de conteúdo diferentes. Sem um método claro, o tempo de estudo acaba sendo distribuído de forma desigual: algumas matérias recebem atenção demais, outras ficam esquecidas até a véspera da prova, gerando estudo de última hora e ansiedade.

**Problema a ser resolvido:** usar IA Generativa para criar um **plano de estudos semanal personalizado**, que organize o tempo disponível do aluno entre as disciplinas cursadas, priorizando de acordo com a proximidade da prova e o nível de dificuldade de cada matéria.

## 2. Metodologia de Execução

1. **Definir o Tema** — problema descrito acima
2. **Criar o Prompt Mestre Inicial** — usando a anatomia profissional de prompt (Persona, Contexto, Tarefa, Formato, Restrições)
3. **Desenvolver 3 Variações** — alterando foco/persona/formato do prompt mestre
4. **Registrar as Respostas** — output do LLM salvo para cada variação
5. **Produzir a Reflexão Crítica** — seção final deste documento

## 3. Técnicas de Prompt Utilizadas

- **Role Prompting** — atribuição de persona (tutor especialista em técnicas de estudo) ao modelo
- **Contexto explícito** — descrição da rotina real do aluno (disciplinas, datas de prova, tempo disponível)
- **Especificação de formato de saída** — pedido de cronograma em tabela
- **Restrições** — carga horária diária máxima, técnicas de estudo específicas (ex: Pomodoro)

## 4. Integrantes do Grupo

- Nome 1
- Nome 2
- Nome 3

---

## 5. Prompt Mestre Inicial

### Anatomia do Prompt

| Elemento | Conteúdo |
|---|---|
| **Persona** | Tutor especialista em técnicas de estudo e produtividade acadêmica |
| **Contexto** | Aluno cursando várias disciplinas ao mesmo tempo, com tempo limitado fora das aulas e provas em datas diferentes |
| **Tarefa** | Criar um cronograma semanal de estudos, priorizando disciplinas por proximidade da prova e nível de dificuldade |
| **Formato** | Tabela com dias da semana, horários, disciplina e tipo de atividade (revisão, exercícios, leitura) |
| **Restrições** | Máximo de 3 horas de estudo por dia útil, usando blocos de 25 minutos (técnica Pomodoro) |

### Prompt

> Você é um tutor especialista em técnicas de estudo e produtividade acadêmica.
>
> Contexto: sou aluno de graduação e curso 4 disciplinas neste semestre:
> - Cálculo I — prova em 10 dias — considero DIFÍCIL
> - Banco de Dados — prova em 20 dias — considero MÉDIA
> - Programação Orientada a Objetos — prova em 15 dias — considero MÉDIA
> - Engenharia de Software — prova em 25 dias — considero FÁCIL
>
> Tenho disponível, de segunda a sexta, 3 horas por dia à noite, e aos sábados 4 horas pela manhã. Domingo não estudo.
>
> Tarefa: monte um cronograma semanal de estudos que distribua meu tempo entre essas 4 disciplinas, priorizando as que têm prova mais próxima e são mais difíceis, sem deixar nenhuma disciplina totalmente sem revisão na semana.
>
> Formato: apresente em uma tabela com colunas Dia, Horário, Disciplina e Tipo de Atividade (ex: revisão de teoria, resolução de exercícios, leitura de material).
>
> Restrições: use blocos de estudo de 25 minutos com 5 minutos de pausa (técnica Pomodoro), sem ultrapassar 3 horas por dia útil e 4 horas no sábado.

### Resposta Obtida

| Dia | Horário | Disciplina | Tipo de Atividade |
|---|---|---|---|
| Segunda | 19h–19h25 / 19h30–19h55 / 20h–20h25 | Cálculo I | Revisão de teoria + resolução de exercícios |
| Segunda | 20h30–20h55 | Banco de Dados | Leitura de material |
| Terça | 19h–19h55 | Cálculo I | Resolução de exercícios |
| Terça | 20h–20h55 | POO | Revisão de teoria |
| Quarta | 19h–19h55 | Cálculo I | Resolução de exercícios |
| Quarta | 20h–20h55 | Banco de Dados | Revisão de teoria |
| Quinta | 19h–19h55 | POO | Resolução de exercícios |
| Quinta | 20h–20h55 | Engenharia de Software | Leitura de material |
| Sexta | 19h–19h55 | Cálculo I | Revisão geral (últimos dias antes da prova) |
| Sexta | 20h–20h55 | Banco de Dados | Resolução de exercícios |
| Sábado | 9h–9h55 | Cálculo I | Simulado / questões de prova anterior |
| Sábado | 10h–10h55 | POO | Revisão de teoria |
| Sábado | 11h–11h55 | Engenharia de Software | Revisão de teoria |

**Observação do modelo:** Cálculo I recebeu mais blocos por ter a prova mais próxima e ser a disciplina mais difícil; Engenharia de Software, por ter prova mais distante e ser considerada fácil, aparece com menos frequência, mas não fica de fora em nenhuma semana.

---

## 6. Variação 1 — Foco Didático

### O que mudou
Mantivemos persona, contexto e restrições, mas alteramos a **tarefa e o formato**: em vez de só entregar o cronograma, pedimos que o modelo explique o raciocínio por trás da distribuição do tempo.

### Prompt

> [Mesma persona e contexto do prompt mestre inicial]
>
> Tarefa: em vez de apenas gerar o cronograma, explique passo a passo o raciocínio usado para decidir quanto tempo dar a cada disciplina. Explique também por que a técnica Pomodoro (blocos de 25 minutos) ajuda na retenção de conteúdo, comparado a estudar horas seguidas sem pausa.
>
> Formato: texto explicativo dividido em tópicos, como se fosse um material de orientação para um aluno que nunca organizou um cronograma de estudos antes.

### Resposta Obtida

**1. Por que Cálculo I recebeu mais tempo**
A prova de Cálculo I é a mais próxima (10 dias) e você mesmo avaliou a disciplina como difícil. Quando um conteúdo é mais complexo e o prazo é curto, o ideal é distribuir revisões em vários dias diferentes, em vez de concentrar tudo perto da prova — isso é chamado de "repetição espaçada" e ajuda a fixar o conteúdo na memória de longo prazo.

**2. Por que Engenharia de Software aparece menos**
Como a prova está mais distante (25 dias) e você considera o conteúdo fácil, não é necessário revisar com a mesma frequência agora. Ainda assim, ela aparece pelo menos uma vez na semana para que o conteúdo não seja esquecido — revisões leves e espaçadas ao longo do tempo funcionam melhor do que estudar tudo de uma vez na última semana.

**3. Por que os sábados têm simulados/questões**
Sábado, com mais tempo disponível (4h), é o melhor momento para praticar questões no formato de prova, porque exige mais concentração contínua do que os blocos de 25 minutos usados nos dias de semana.

**4. Por que usar blocos de 25 minutos (Pomodoro)?**
Estudar por longos períodos sem pausa reduz a capacidade de concentração com o tempo — depois de um tempo, o cérebro passa a "ler sem absorver". Blocos curtos com pausas de 5 minutos mantêm o nível de atenção mais alto durante todo o período de estudo, e as pausas ajudam o cérebro a consolidar o que acabou de ser estudado antes de seguir para o próximo bloco.

---

## 7. Variação 2 — Foco em Otimização de Tempo

### O que mudou
Mantivemos persona e contexto, mas adicionamos uma **restrição extra**: um imprevisto reduziu o tempo disponível do aluno, e pedimos ao modelo que otimize a distribuição diante dessa limitação.

### Prompt

> [Mesma persona e contexto do prompt mestre inicial]
>
> Tarefa: nesta semana, um imprevisto reduziu meu tempo disponível: só tenho 1h30 por dia de segunda a sexta (em vez de 3h), e não terei o sábado disponível. Refaça o cronograma priorizando o que é estrategicamente mais importante, e explique o que você decidiu cortar ou reduzir e por quê.
>
> Restrições adicionais:
> - Priorize sempre a disciplina com prova mais próxima
> - Não elimine completamente nenhuma disciplina da semana
> - Indique claramente o que foi reduzido em relação ao cronograma original

### Resposta Obtida

| Dia | Horário | Disciplina | Tipo de Atividade |
|---|---|---|---|
| Segunda | 19h–19h55 | Cálculo I | Revisão de teoria + exercícios |
| Terça | 19h–19h55 | Cálculo I | Resolução de exercícios |
| Quarta | 19h–19h55 | Banco de Dados | Revisão de teoria |
| Quinta | 19h–19h55 | Cálculo I | Simulado curto |
| Sexta | 19h–19h55 | POO | Revisão de teoria |

**O que foi cortado e por quê:**
- **Sábado inteiro removido**, já que não está mais disponível — os 4h de simulados que estavam lá (Cálculo I, POO e Eng. de Software) tiveram que ser redistribuídos ou reduzidos.
- **Engenharia de Software saiu do cronograma desta semana**, pois é a disciplina com prova mais distante (25 dias) e nível fácil — é a que pode esperar mais uma semana sem revisão sem grande prejuízo.
- **Cálculo I manteve 3 dos 5 dias**, porque continua sendo a prioridade máxima (prova mais próxima + maior dificuldade).
- **Banco de Dados e POO foram reduzidos a apenas 1 dia cada**, o mínimo necessário para não ficarem totalmente esquecidas.

**Alerta do modelo:** com apenas 1h30/dia, o ideal é, assim que o tempo normal voltar, repor ao menos uma sessão extra de Engenharia de Software para compensar a semana sem revisão.

---

## 8. Variação 3 — Foco em Persona (Aluno calouro)

### O que mudou
Trocamos a **persona de destino** (para quem a resposta é escrita) e o **formato**: pedimos que a explicação seja feita para um calouro que nunca organizou uma rotina de estudos sozinho, sem termos técnicos de produtividade.

### Prompt

> [Mesma persona (quem responde) e contexto do prompt mestre inicial]
>
> Tarefa: explique como funciona esse cronograma de estudos para um calouro do primeiro semestre, que está tendo que organizar os estudos sozinho pela primeira vez na vida (sem a rotina fixa do ensino médio) e nunca ouviu falar em técnica Pomodoro ou repetição espaçada.
>
> Formato: texto simples e acolhedor, sem jargão de produtividade, explicando por que dividir o tempo entre as matérias é melhor do que estudar uma matéria por vez até terminar.
>
> Restrições: no máximo 150 palavras.

### Resposta Obtida

No ensino médio, alguém montava seu horário por você. Agora, na faculdade, essa organização é sua responsabilidade — e é normal sentir que o tempo nunca é suficiente para tudo.

Uma armadilha comum é focar só na matéria que está "pegando fogo" e deixar as outras de lado até a última hora. O problema é que, quando chegar a vez delas, você vai estar correndo contra o tempo também.

Por isso, este cronograma divide seus dias entre as disciplinas, dando mais atenção para a prova mais próxima, mas sem esquecer totalmente as outras. Estudar um pouquinho de cada uma, várias vezes na semana, funciona melhor do que estudar uma matéria inteira de uma vez só — seu cérebro absorve e lembra melhor assim.

---

## 9. Reflexão Crítica

### 9.1 Análise Crítica — O que funcionou e o que faltou

**O que funcionou:**
- O prompt mestre, por já trazer contexto detalhado (disciplinas, datas de prova, nível de dificuldade e tempo disponível), gerou um cronograma coerente e realista, respeitando as restrições de tempo impostas.
- As variações mostraram como o mesmo problema pode ser abordado de formas bem diferentes: explicação pedagógica, replanejamento sob restrição de tempo, e comunicação simplificada para um público iniciante.

**O que faltou / limitações observadas:**
- O prompt mestre inicial não pediu folgas ou dias de descanso extra — o modelo preencheu praticamente todos os dias úteis, o que pode não ser sustentável em semanas com outras responsabilidades (trabalhos, provas de outras matérias não mencionadas).
- Não foi pedido ao modelo indicar *fontes de estudo* (livro, lista de exercícios, videoaula) — o cronograma diz "o quê" estudar, mas não "com que material".
- A avaliação de dificuldade de cada disciplina (fácil/médio/difícil) foi informada pelo próprio aluno de forma subjetiva; o modelo não tem como validar se essa percepção está correta.

### 9.2 Prompt Refinado

Combinando os aprendizados das 3 variações, o prompt mestre ficaria assim numa segunda iteração:

> Você é um tutor especialista em técnicas de estudo e produtividade acadêmica.
>
> Contexto: [mesmas disciplinas, prazos e dificuldades do prompt original], com a mesma disponibilidade de horários.
>
> Tarefa: monte um cronograma semanal de estudos que:
> 1. Priorize disciplinas por proximidade da prova e dificuldade;
> 2. Inclua pelo menos 1 dia completo de descanso na semana;
> 3. Sugira, para cada bloco de estudo, um tipo de material recomendado (ex: lista de exercícios, resumo teórico, videoaula);
> 4. Ao final, explique em linguagem simples por que essa distribuição foi escolhida, como se estivesse explicando para um calouro.
>
> Formato: tabela (Dia, Horário, Disciplina, Atividade, Material sugerido) seguida de um parágrafo explicativo.
>
> Restrições: blocos de 25 minutos com pausa de 5 (Pomodoro), máximo de 3h/dia útil e 4h no sábado, domingo livre.

### 9.3 Comparação entre Resultado Inicial e Refinado

| Aspecto | Prompt Inicial | Prompt Refinado |
|---|---|---|
| Dia de descanso | Não previsto — todos os dias úteis ocupados | Explicitamente garantido |
| Material de estudo | Não indicado | Sugerido por bloco |
| Explicação do raciocínio | Só apareceu quando pedimos na Variação 1 | Já incorporada ao final do cronograma |
| Adaptação a imprevistos | Só apareceu quando pedimos na Variação 2 | Ainda precisaria ser pedida à parte (limitação que permanece) |

O prompt refinado cobre mais necessidades de uma vez, mas a adaptação a imprevistos de última hora continua sendo melhor tratada como um pedido separado, já que depende de uma situação que muda a cada semana.

### 9.4 Validação — Como as respostas foram conferidas por humanos

- A distribuição de tempo entre disciplinas foi conferida manualmente pelo grupo, somando as horas de cada matéria na semana para garantir que batiam com o limite de 3h/dia (ou 1h30 na Variação 2) informado no prompt.
- A lógica de priorização (prova mais próxima + maior dificuldade = mais tempo) foi validada comparando o cronograma gerado com o senso comum de técnicas de estudo já conhecidas pelo grupo (repetição espaçada, técnica Pomodoro).
- Nenhuma informação sobre conteúdo específico das disciplinas foi gerada pelo modelo (ele não "inventou" matéria de Cálculo ou Banco de Dados), reduzindo o risco de erro factual nas respostas.

---
*Atividade Prática A2 — Fundamentos de AI e Engenharia de Prompt.*
