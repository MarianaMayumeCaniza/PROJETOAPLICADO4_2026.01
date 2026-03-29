<p align="center">
  <img src="Assets_Figures/logo-mackenzie.png" width="180"/>
</p>

<h1 align="center">UNIVERSIDADE PRESBITERIANA MACKENZIE</h1>

<h2 align="center">PROJETO APLICADO IV — Ciência de Dados EaD</h2>
<h3 align="center">2026.01</h3>

---

<h2 align="center">
Indústria 4.0 Predictive: Modelagem de Séries Temporais para Otimização de Infraestrutura e Produção Sustentável
</h2>

---

<div align="right">

Projeto elaborado para a disciplina Projeto Aplicado IV, do curso de Ciência de Dados da Universidade Presbiteriana Mackenzie, na categoria Projeto Extensionista, como requisito parcial para aprovação. <br>
Orientador: profº Gustavo Scalabrini Sampaio

</div>

---

<p align="center">
<strong>Grupo 7</strong><br>
Amarildo Maciel Junior — 10441652<br>
Mariana Mayume Caniza — 10290174<br>
Stella Amaral de Campos — 10441310
</p>

---

<p align="center">
São Paulo,<br>
2026
</p>

---

<br>
# 📑 Sumário

- [1. Introdução](#INTRODUÇÃO)
- [2. Motivação e Justificativa](#MOTIVAÇÃO_E_JUSTIFICATIVA)
  - [2.1 ODS 9 – Indústria, Inovação e Infraestrutura](#ods-9--indústria-inovação-e-infraestrutura)
  - [2.2 ODS 12 – Consumo e Produção Responsáveis](#ods-12--consumo-e-produção-responsáveis)
  - [2.3 Potencial de Aplicabilidade](#potencial-de-aplicabilidade)
- [3. Objetivo](#objetivo)
- [4. Metodologia e Base de dados](#descrição-da-base-de-dados)
  - [4.1 Fonte dos Dados](#fonte-dos-dados)
  - [4.2 Informações Disponíveis](#informações-disponíveis)
  - [4.3 Ferramentas e Ambiente de Desenvolvimento](#estrutura-e-organização)
  - [4.4 EDA](#período-de-coleta)
- [Referências](#referências)

---

# 1. INTRODUÇÃO

O presente projeto desenvolve-se no contexto da Ciência de Dados aplicada à Economia Industrial. Conforme define Fernandes (2026), uma série temporal caracteriza-se como um conjunto de observações ordenadas no tempo, coletadas em intervalos regulares, permitindo a análise de fenômenos que evoluem cronologicamente. Tais séries são fundamentais em diversas áreas, como a Economia, pois possibilitam não apenas descrever o comportamento de uma variável, mas também prever valores futuros e auxiliar no controle de processos.
Neste trabalho, o foco recai sobre o Índice de Produção Física Industrial (PIM-PF), um indicador vital para medir o dinamismo econômico de um país. A análise de séries temporais permite identificar elementos característicos como a tendência (que indica a propensão de crescimento ou declínio a longo prazo) e a sazonalidade, que revela padrões de variação que se repetem em intervalos fixos. O problema central reside na volatilidade da produção industrial brasileira, que impõe desafios severos aos gestores de infraestrutura. Sem uma análise preditiva robusta, o setor enfrenta riscos de subutilização de recursos ou gargalos logísticos, gerando incertezas que dificultam a construção de uma infraestrutura resiliente.


---

# 2. MOTIVAÇÃO E JUSTIFICATIVA

A motivação para este estudo surge da identificação de uma lacuna crítica no planejamento industrial brasileiro: a dificuldade em antecipar flutuações sazonais e ciclos econômicos que impactam diretamente a cadeia de suprimentos. Frequentemente, a falta de ferramentas analíticas acessíveis para a previsão de demanda resulta em uma produção descalibrada, onde o "ruído" ou erro aleatório da série é confundido com mudanças estruturais, levando a decisões equivocadas de investimento. Esta oportunidade de melhoria no planejamento logístico é o que impulsiona a proposição de um produto analítico focado em previsibilidade.
A justificativa do projeto apresenta contribuições em duas frentes principais. Do ponto de vista técnico, a aplicação de modelos de decomposição clássica e projeção estatística oferece uma base científica para a tomada de decisão, transformando dados brutos em inteligência estratégica. Socialmente, o projeto alinha-se aos Objetivos de Desenvolvimento Sustentável (ODS) da ONU.


## 2.1 ODS 9 – Indústria, Inovação e Infraestrutura

A capacidade de prever a produção permite que a infraestrutura logística e energética do país seja planejada com maior precisão, evitando colapsos em períodos de alta demanda.

## 2.2 ODS 12 – Consumo e Produção Responsáveis

Ao identificar padrões sazonais, as indústrias podem ajustar seu estoque e produção, reduzindo desperdícios de matéria-prima e promovendo uma produção mais consciente.

## 2.3 Potencial de Aplicabilidade

A solução proposta consiste em um produto analítico baseado em modelos estatísticos de séries temporais que funcionará como uma ferramenta de auxílio à tomada de decisão para associações industriais e gestores governamentais, permitindo antecipar flutuações de mercado e otimizar a alocação de recursos financeiros e humanos.

---

# 3. OBJETIVO

O objetivo deste projeto é desenvolver um produto analítico baseado em um modelo preditivo univariado para o índice de produção industrial brasileira, visando otimizar a gestão de recursos e infraestrutura. Para isso, o grupo realizará a decomposição clássica da série para isolar seus componentes de tendência, sazonalidade e ruído, classificando-a quanto à sua estacionaridade e linearidade conforme os preceitos estatísticos de Morettin e Toloi (2018). Ao final, o projeto busca projetar valores futuros que sirvam de subsídio para o planejamento estratégico do cliente, focando na mitigação de custos operacionais e na redução de desperdícios produtivos.


---

# 4. METODOLOGIA E BASE DE DADOS

  A base de dados utilizada provém da plataforma Sistema IBGE de Recuperação Automática (SIDRA), mantida pelo Instituto Brasileiro de Geografia e Estatística (IBGE), especificamente da Tabela 8159, que detalha a Pesquisa Industrial Mensal - Produção Física (PIM-PF). 
  Os dados consistem em um número-índice da produção física industrial, utilizando uma base fixa mensal (2012 = 100) sem ajuste sazonal. Essa característica é imprescindível para que o grupo possa realizar a identificação de padrões repetitivos e a Decomposição Clássica da série em seus componentes de tendência, sazonalidade e ruído.
  
## 4.1 Fonte dos Dados

Pesquisa Industrial Mensal – Produção Física (PIM-PF) – Tabela 8159.

## 4.2 Informações Disponíveis
Abrangência Geográfica: Unidade Federativa Brasil (Total Nacional).
Periodicidade: Mensal, abrangendo o período de Janeiro de 2006 a Dezembro de 2022 (n=204).
Atributos: A base utiliza a Classificação Nacional de Atividades Econômicas (CNAE 2.0), permitindo a extração de dados da "Indústria Geral" ou futuras expansões para segmentos específicos.
Forma de Coleta: Coleta administrativa e censitária realizada mensalmente pelo IBGE junto às unidades produtivas.

## 4.3 Ferramentas e Ambiente de Desenvolvimento
A manipulação e modelagem dos dados serão realizadas utilizando a linguagem Python 3.x em ambiente Jupyter Notebook. As principais bibliotecas aplicadas são:
Pandas e Numpy: Para estruturação da série e tratamento de dados.
Matplotlib e Seaborn: Para a Análise Exploratória de Dados (EDA) e visualização gráfica.
Statsmodels: Para a realização da Decomposição Sazonal, Testes de Estacionariedade (ADF) e futura implementação de modelos ARIMA/SARIMA.

## 4.4 EDA
O processo de investigação analítica segue o seguinte fluxo de trabalho:Pré-processamento: Conversão dos dados do formato Wide para Long e tratamento da tipagem temporal (datetime).Análise de Estacionariedade: Aplicação do teste de raiz unitária (Augmented Dickey-Fuller) para verificar se a série exige diferenciação.Decomposição Sazonal: Separação estatística da Tendência ($T_t$) e Sazonalidade ($S_t$), validando a escolha da periodicidade mensal para capturar os ciclos produtivos anuais.Levantamento de Técnicas: Definição de modelos de suavização exponencial (Holt-Winters) e modelos autorregressivos para a fase de predição.


---

# Referências

BRASIL. Instituto Brasileiro de Geografia e Estatística.  
**Pesquisa Industrial Mensal – Produção Física (PIM-PF): Tabela 8159.**  
Rio de Janeiro: IBGE, 2023.  
Disponível em: https://sidra.ibge.gov.br/tabela/8159.  
Acesso em: 28 fev. 2026.

FERNANDES, Leandro Carlos.  
Projeto Aplicado IV: Aula 1 – Introdução às Séries Temporais.  
São Paulo: Universidade Presbiteriana Mackenzie, 2026. Texto de apoio.

MORETTIN, P. A.; TOLOI, C. M. C.  
Análise de séries temporais. 3. ed. São Paulo: Blucher, 2018. v. 1.

ORGANIZAÇÃO DAS NAÇÕES UNIDAS.  
Objetivos de Desenvolvimento Sustentável: ODS 9 e ODS 12.  
Disponível em: https://brasil.un.org/pt-br/sdgs.  
Acesso em: 28 fev. 2026.
