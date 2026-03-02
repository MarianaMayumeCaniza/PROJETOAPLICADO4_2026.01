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

|                     |                                                                 |
|---------------------|-----------------------------------------------------------------|
|                     | Projeto elaborado para a disciplina Projeto Aplicado IV, do curso de Ciência de Dados da Universidade Presbiteriana Mackenzie, na categoria Projeto Extensionista, como requisito parcial para aprovação. |

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

---

# 📑 Sumário

- [Introdução](#introdução)
  - [Problema](#problema)
- [Motivação e Justificativa](#motivação-e-justificativa)
  - [ODS 9 – Indústria, Inovação e Infraestrutura](#ods-9--indústria-inovação-e-infraestrutura)
  - [ODS 12 – Consumo e Produção Responsáveis](#ods-12--consumo-e-produção-responsáveis)
  - [Potencial de Aplicabilidade](#potencial-de-aplicabilidade)
- [Objetivo](#objetivo)
  - [Objetivo Geral](#objetivo-geral)
  - [Objetivos Específicos](#objetivos-específicos)
- [Descrição da Base de Dados](#descrição-da-base-de-dados)
  - [Fonte dos Dados](#fonte-dos-dados)
  - [Informações Disponíveis](#informações-disponíveis)
  - [Estrutura e Organização](#estrutura-e-organização)
  - [Período de Coleta](#período-de-coleta)
  - [Forma de Coleta](#forma-de-coleta)
- [Referências](#referências)

---

# Introdução

O presente projeto desenvolve-se no contexto da Ciência de Dados aplicada à Economia Industrial. De acordo com Fernandes (2026), uma série temporal é um conjunto de observações ordenadas no tempo e coletadas em intervalos regulares.

Neste trabalho, o foco recai sobre o Índice de Produção Física Industrial (PIM-PF), um indicador vital para medir o dinamismo econômico de um país.

## Problema

A volatilidade da produção industrial brasileira apresenta um desafio para os gestores de infraestrutura e produção. Sem uma análise preditiva, a indústria enfrenta o risco de subutilização de recursos ou gargalos logísticos.

O problema selecionado é a incerteza no planejamento produtivo, que muitas vezes leva ao desperdício de insumos e energia, dificultando a construção de uma infraestrutura resiliente e sustentável.

---

# Motivação e Justificativa

A relevância deste tema fundamenta-se nos Objetivos de Desenvolvimento Sustentável (ODS) da Organização das Nações Unidas (ONU).

## ODS 9 – Indústria, Inovação e Infraestrutura

A capacidade de prever a produção permite que a infraestrutura logística e energética do país seja planejada com maior precisão, evitando colapsos em períodos de alta demanda.

## ODS 12 – Consumo e Produção Responsáveis

Ao identificar padrões sazonais, as indústrias podem ajustar seu estoque e produção, reduzindo desperdícios de matéria-prima e promovendo uma produção mais consciente.

## Potencial de Aplicabilidade

A solução proposta consiste em um produto analítico baseado em modelos estatísticos de séries temporais, que funcionará como uma ferramenta de auxílio à tomada de decisão para associações industriais e gestores governamentais.

Essa solução permitirá antecipar flutuações de mercado e otimizar a alocação de recursos financeiros e humanos.

---

# Objetivo

## Objetivo Geral

Desenvolver um modelo preditivo univariado para o índice de produção industrial brasileira.

## Objetivos Específicos

- Realizar a decomposição clássica da série temporal para isolar tendência, sazonalidade e ruído.
- Classificar a série quanto à sua estacionariedade e linearidade.
- Projetar valores futuros que sirvam de subsídio para o planejamento estratégico do cliente.
- Contribuir para a redução de custos operacionais e desperdícios.

---

# Descrição da Base de Dados

O projeto utilizará dados secundários oficiais obtidos via plataforma SIDRA do Instituto Brasileiro de Geografia e Estatística.

## Fonte dos Dados

Pesquisa Industrial Mensal – Produção Física (PIM-PF) – Tabela 8159.

## Informações Disponíveis

Número-índice da produção física industrial (base fixa mensal sem ajuste sazonal).

## Estrutura e Organização

Trata-se de uma série univariada, organizada de forma cronológica mensal.

## Período de Coleta

Janeiro de 2006 a dezembro de 2022 (série encerrada conforme atualização do IBGE para a nova base de 2012).

## Forma de Coleta

Coleta administrativa e censitária realizada mensalmente pelo IBGE junto a unidades produtivas.

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
