# 📒 Caderno Temático — Tesouro Direto
> Desafio de Projeto | DIO — Uso do NotebookLM como ferramenta de aprendizagem ativa

---

## 1. Contexto e Objetivos

### Por que Tesouro Direto?
Escolhi o Tesouro Direto por ser um dos investimentos mais acessíveis e seguros do Brasil, porém ainda pouco compreendido por jovens e iniciantes em finanças. Como estudante de Sistemas de Informação no início da graduação, entendo que educação financeira é tão essencial quanto educação tecnológica — e o Tesouro Direto é um ponto de partida ideal para quem quer começar a investir com segurança.

### Objetivos de Estudo
- Compreender o que é o Tesouro Direto e como ele funciona
- Conhecer os tipos de títulos disponíveis e suas diferenças
- Entender como funciona o rendimento na prática
- Identificar os erros mais comuns de iniciantes
- Construir um glossário dos principais termos do tema

---

## 2. Curadoria de Fontes

Foram selecionadas **7 fontes abertas** e carregadas no NotebookLM:

| # | Tipo | Fonte |
|---|---|---|
| 1 | 🎥 Vídeo | [YouTube — Introdução ao Tesouro Direto](https://www.youtube.com/watch?v=3-5Ujc5dyhE) |
| 2 | 🎥 Vídeo | [YouTube — Como investir no Tesouro Direto](https://www.youtube.com/watch?v=y2sBkIX72-g) |
| 3 | 🎥 Vídeo | [YouTube — Tipos de títulos do Tesouro Direto](https://www.youtube.com/watch?v=OOEssu7j5UQ) |
| 4 | 📄 PDF | [Guia Fácil Tesouro Direto — André Massaro (2015)](https://www.andremassaro.com.br/wp-content/uploads/2020/06/Guia-Facil-Tesouro-Direto-Andre-Massaro-2015.pdf) |
| 5 | 📄 PDF | [Artigo Acadêmico — Uninove (2013)](http://docs.uninove.br/arte/fac/publicacoes/pdf/v4-n1-2013/Ana_Bruna.pdf) |
| 6 | 📄 PDF | [Guia de Produto Tesouro Direto — Agora Invest](https://agorainvest.com.br/uploads/ns/pdf/prodtesourodireto.pdf) |
| 7 | 📄 PDF | [Manual do App Tesouro Direto — Governo Federal](https://www.gov.br/tesouronacional/pt-br/importacao-arquivos/Manual-do-app-do-tesouro-direto.pdf) |

---

## 3. Engenharia de Prompts e Cicatrizes

Abaixo estão documentados todos os prompts testados, as respostas obtidas, as fontes utilizadas pelo NotebookLM e a análise crítica de cada interação.

---

### 🔹 Prompt 1 — Conceito básico

**Pergunta inicial:**
> "O que é tesouro direto?"

**Problema encontrado:**
A resposta trouxe o conceito correto, mas o NotebookLM foi além do que foi perguntado, adicionando informações não solicitadas. A resposta útil representou apenas cerca de 1/5 do total entregue.

**Prompt reformulado:**
> "Me diga exatamente o que é tesouro direto, quero saber apenas o conceito em um parágrafo simples, somente."

**Resposta obtida:**
> O Tesouro Direto é um programa criado em 2002 pelo Tesouro Nacional, em parceria com a B3, que permite a pessoas físicas a compra de títulos públicos federais diretamente através da internet. Na prática, ao adquirir um título, o investidor está emprestando dinheiro para o Governo Federal financiar a dívida pública e realizar investimentos em áreas como saúde e educação, recebendo em troca o valor aplicado acrescido de juros em uma data futura. Este programa é considerado o investimento de menor risco e maior segurança do Brasil, pois os títulos possuem garantia integral do próprio Tesouro Nacional.

**Fontes utilizadas:** 1 fonte (vídeo do YouTube)

**Análise:**
O prompt reformulado resolveu o problema. A lição aprendida foi que delimitar o formato da resposta ("apenas o conceito", "em um parágrafo", "somente") é essencial para obter respostas diretas e sem ruído.

---

### 🔹 Prompt 2 — Tipos de títulos

**Pergunta:**
> "Quais são os tipos de títulos disponíveis no Tesouro Direto e qual a diferença entre eles?"

**Resposta obtida:**
Os títulos são classificados por forma de remuneração: prefixados, pós-fixados ou híbridos.

- **Tesouro Selic (Pós-fixado):** Acompanha a taxa básica de juros da economia. Baixa volatilidade, ideal para reserva de emergência.
- **Tesouro Prefixado:** Taxa de juros fixa definida na compra. Ideal quando se espera queda nos juros, porém sujeito à marcação a mercado.
- **Tesouro IPCA+ (Híbrido):** Combina taxa fixa com variação da inflação. Protege o poder de compra no longo prazo.
- **Tesouro Renda+ (Híbrido):** Focado em aposentadoria. Após período de acumulação, devolve o patrimônio em 240 parcelas mensais corrigidas pela inflação.

Diferença na forma de pagamento:
- **Títulos "Principal":** Pagamento único no vencimento.
- **Títulos com Juros Semestrais:** Pagam cupons a cada seis meses, mas antecipam o Imposto de Renda.

**Fontes utilizadas:** Todas as 7 fontes

**Análise:**
A resposta foi completa, porém o NotebookLM detalhou cada tipo mesmo sem ser solicitado explicitamente. Para este caso, o comportamento foi aceitável pois o objetivo era justamente entender as diferenças. Não foi necessário reformular.

---

### 🔹 Prompt 3 — Rendimento na prática

**Pergunta:**
> "Se eu investir R$ 1.000 no Tesouro Selic hoje, como funciona o rendimento? Explique de forma simples, sem voltas."

**Resposta obtida:**
- **Rentabilidade Pós-fixada:** O dinheiro acompanha a taxa Selic. Se ela subir, rende mais; se cair, rende menos.
- **Ganhos Diários:** Diferente da poupança, o Tesouro Selic rende todos os dias úteis.
- **Segurança do Principal:** Em caso de resgate antecipado, o investidor não corre risco de receber menos que os R$ 1.000 investidos.
- **Cálculo Final:** No resgate, o investidor recebe os R$ 1.000 acrescidos de toda a variação da Selic do período.

**Fontes utilizadas:** 6 das 7 fontes

**Análise:**
Melhor resposta obtida até então. A instrução "sem voltas" funcionou bem para eliminar informações desnecessárias. O NotebookLM foi direto ao ponto e a resposta ficou fácil de compreender.

---

### 🔹 Prompt 4 — Erros comuns

**Pergunta:**
> "Quais são os erros mais comuns de quem está começando a investir no Tesouro Direto?"

**Resposta obtida:**
- Ignorar a marcação a mercado
- Escolher o título errado para reserva de emergência
- Optar por juros semestrais sem necessidade de renda imediata
- Falta de constância nos aportes mensais
- Não ter objetivos definidos antes de investir
- Falta de diversificação na carteira
- Começar a planejar a aposentadoria muito tarde

**Fontes utilizadas:** Todas as 7 fontes

**Análise:**
Percebeu-se uma evolução clara no comportamento do NotebookLM ao longo das perguntas — as respostas foram ficando progressivamente mais diretas e objetivas. Nenhuma reformulação foi necessária.

---

### 🔹 Prompt 5 — Glossário

**Pergunta:**
> "Liste apenas os principais termos do Tesouro Direto com uma explicação bem simples para cada um deles."

**Resposta obtida:**
Glossário completo com 16 termos (ver seção 4 abaixo).

**Fontes utilizadas:** Todas as 7 fontes

**Análise:**
A resposta foi extensa, porém adequada ao objetivo. Cada termo recebeu uma explicação direta e acessível para iniciantes. A palavra "apenas" no prompt ajudou a evitar parágrafos explicativos longos.

---

## 4. Miniguia de Estudo

### 📌 Resumos Estruturados

#### O que é o Tesouro Direto?
O Tesouro Direto é um programa do Governo Federal criado em 2002, em parceria com a B3, que permite a qualquer pessoa física comprar títulos públicos pela internet. Ao investir, o cidadão empresta dinheiro ao governo, que usa esses recursos para financiar áreas como saúde e educação. Em troca, recebe o valor investido de volta com juros em uma data futura. É considerado o investimento mais seguro do Brasil, com garantia integral do Tesouro Nacional.

#### Tipos de Títulos
Os títulos são divididos em três categorias conforme a forma de remuneração:

- **Pós-fixado (Tesouro Selic):** Ideal para reserva de emergência. Segue a taxa Selic e tem baixa volatilidade.
- **Prefixado (Tesouro Prefixado):** A taxa é definida na compra. Bom quando se espera queda nos juros futuros.
- **Híbrido (Tesouro IPCA+ e Tesouro Renda+):** Combina taxa fixa com proteção contra a inflação. Indicado para objetivos de longo prazo e aposentadoria.

#### Como funciona o rendimento?
O rendimento varia conforme o título escolhido. No Tesouro Selic, por exemplo, o dinheiro cresce diariamente acompanhando os juros básicos da economia. No Tesouro Prefixado, a taxa é conhecida desde o início. No Tesouro IPCA+, o ganho é a soma de uma taxa fixa com a inflação do período.

#### Principais cuidados para iniciantes
- Usar o Tesouro Selic para a reserva de emergência
- Não vender títulos prefixados antes do vencimento em momentos de alta dos juros
- Manter constância nos aportes mensais
- Definir objetivos antes de escolher o título
- Evitar títulos com juros semestrais se o objetivo for acumulação de longo prazo

---

### 📖 Glossário

| Termo | Definição simples |
|---|---|
| **Tesouro Direto** | Programa do governo que permite comprar títulos públicos pela internet |
| **Títulos Públicos** | Certificados de dívida do governo; ao comprá-los, você empresta dinheiro ao Estado |
| **Renda Fixa** | Categoria de investimento onde as regras de rendimento são definidas na aplicação |
| **Vencimento** | Data em que o governo devolve o valor investido com juros |
| **Agente de Custódia** | Banco ou corretora que intermedia suas operações no Tesouro Direto |
| **Marcação a Mercado** | Variação diária do preço do título conforme as mudanças nas taxas de juros |
| **Taxa Selic** | Taxa básica de juros da economia brasileira, definida pelo Banco Central |
| **IPCA** | Índice oficial que mede a inflação no Brasil |
| **Tesouro Selic (LFT)** | Título pós-fixado que acompanha a Selic; indicado para reserva de emergência |
| **Tesouro Prefixado (LTN)** | Título com taxa de juros fixa definida na compra |
| **Tesouro IPCA+ (NTN-B)** | Título híbrido que paga taxa fixa mais inflação, protegendo o poder de compra |
| **Tesouro Renda+** | Título focado em aposentadoria; devolve o montante em 240 parcelas mensais |
| **Juros Semestrais (Cupom)** | Opção de título que paga rendimentos na conta a cada seis meses |
| **Liquidez** | Rapidez com que o título pode ser convertido em dinheiro |
| **Alíquota Regressiva** | Regra do IR onde a taxa sobre o lucro diminui com o tempo (de 22,5% a 15%) |
| **P.U. (Preço Unitário)** | Valor de mercado de um título inteiro no momento da compra |

---

### 🔁 Prompts Reutilizáveis

Use estes prompts em futuras revisões sobre Tesouro Direto ou adapte para outros temas financeiros:

```
1. "Me diga exatamente o que é [tema], quero saber apenas o conceito 
   em um parágrafo simples, somente."

2. "Quais são os tipos de [produto/investimento] disponíveis 
   e qual a diferença entre eles?"

3. "Se eu investir R$ [valor] em [título] hoje, como funciona 
   o rendimento? Explique de forma simples, sem voltas."

4. "Quais são os erros mais comuns de quem está começando 
   a investir em [tema]?"

5. "Liste apenas os principais termos de [tema] com uma explicação 
   bem simples para cada um deles."

6. "Compare [opção A] e [opção B] em uma tabela com as principais 
   diferenças e para qual perfil cada um é mais indicado."

7. "Resuma os principais conceitos de [tema] para alguém que nunca 
   investiu antes, em no máximo 5 tópicos."
```

---

## 5. Conclusão

Este caderno temático demonstrou que o NotebookLM é uma ferramenta poderosa para estudo ativo quando bem utilizado. A principal lição aprendida foi que **a qualidade da pergunta determina diretamente a qualidade da resposta** — prompts vagos geram respostas genéricas, enquanto prompts específicos e bem delimitados geram respostas precisas e úteis.

Ao longo dos testes, ficou evidente uma evolução no comportamento da IA: as respostas foram progressivamente mais diretas conforme os prompts foram refinados, mostrando que a engenharia de prompts é uma habilidade que se desenvolve com prática e observação crítica.

---

*Projeto desenvolvido como parte do desafio prático da [DIO — Digital Innovation One](https://www.dio.me)*
