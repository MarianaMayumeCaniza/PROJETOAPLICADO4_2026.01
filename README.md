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
### 4.3.1 Procedimento de Coleta e Reprodutibilidade
A estratégia de coleta de dados deste projeto foi estruturada de forma híbrida para garantir tanto a segurança quanto a reprodutibilidade técnica:
1.  **Armazenamento Local (Backup):** Os dados brutos foram extraídos manualmente do portal SIDRA/IBGE (Tabela 8159): [https://sidra.ibge.gov.br/tabela/8159](https://sidra.ibge.gov.br/tabela/8159)  e armazenados no diretório local `BaseDeDados`. Esse procedimento serve como uma backup para a integridade dos dados originais.
2. **Automação via API:** Para o processamento e análise no ambiente Python, foi utilizada a **API (Application Programming Interface)** do sistema SIDRA. Diferente da coleta manual, o uso de requisições diretas ao *endpoint* do IBGE permite que a série seja extraída com a mesma configuração de filtros de forma automática. A URL de requisição [`(https://apisidra.ibge.gov.br/values/t/8159/n[NIVEL]/[TERRITORIO]/v/[VARIAVEL]/p/[PERIODO]/c544/[SETOR]/d/v[VARIAVEL]%205)`] é composta por parâmetros técnicos que definem os filtros da análise, exemplo:

[https://apisidra.ibge.gov.br/values/t/8159/n1/all/v/11599/p/all/c544/129314/d/v11599%205]
| Parâmetro | Código | Descrição Técnica |
| :--- | :--- | :--- |
| **Tabela** | `/t/8159` | Identificador da Pesquisa Industrial Mensal (PIM-PF) |
| **Variável** | `/v/11599` | Seleção do "Índice de base fixa (2012=100)"|
| **Classificação** | `/c544/129314` | Filtro para o segmento de "Indústria Geral" |
| **Período** | `/p/all` |Extração da série histórica completa disponível |
| **Nível Territorial** | `/n1/all` | Filtro para o total nacional (Brasil) |

### 4.3.2 Dimensões de Análise e Níveis de Detalhamento
Para realizar uma análise profunda que parte do panorama nacional para as especificidades setoriais e regionais, foram definidos recortes principais de estudo (subamostras):
| Dimensão de Análise | Objetivo Técnico | Período | Abrangência | Variável Principal |
| :--- | :--- | :--- | :--- | :--- |
| **Panorama Geral (Macro)** | Identificar tendência e sazonalidade de longo prazo| 2002 – 2022 | Brasil | Número-índice |
| **Dinâmica de Momentum (EVM)** | Analisar a volatilidade e choques de curto prazo mês a mês| 2002 – 2022 | Brasil | Variação Mensal |
| **Ciclo Econômico (AVA)** | Observar o crescimento real acumulado, removendo o "ruído" mensal | 2002 – 2022 | Brasil | Acumulada no Ano |
| **Recorte Regional** | Comparar o desempenho da produção em polos específicos (ex: Sudeste) | 2022 | Sudeste | Número-índice |
| **Recorte Setorial** | Avaliar como nichos específicos reagem a crises (ex: Bebidas) | 2002 – 2022 | Bebidas | Número-índice |
| **Janela de Eventos (Zoom)** | Investigar comportamentos atípicos em períodos de alta volatilidade | Jul – Dez/2022 | Brasil | EVM |

Esta estrutura modular permite verificar se padrões identificados no nível nacional se mantêm ou se alteram em contextos regionais e setoriais específicos.



## 4.4 Pré-processamento

### 4.4.1 Transformar em Data
Conversão de Formato: A coluna de meses foi convertida para o formato datetime, estabelecendo a cronologia correta da série. 

Frequência Mensal (asfreq): Utilizou-se a função asfreq('MS') para garantir a continuidade temporal. Este passo "carimba" o calendário, assegurando que não existam saltos entre os meses, o que é um pré-requisito para o funcionamento de modelos como o SARIMA.

### 4.4.2 Integridade de Dados: Faltantes e Duplicadas

Interpolação Linear: Caso o asfreq identifique meses ausentes (vazios), aplica-se a função interpolate(). Em vez de usar zero — o que distorceria as médias — a interpolação faz a media em meio termo entre meses vizinhos para preencher o ponto , mantendo a suavidade da série.

Tratamento de Duplicadas: Foi realizada uma "batida policial" no índice para detectar datas repetidas. Por segurança, caso existam duplicatas, mantém-se o primeiro registro (keep='first') para garantir que cada mês seja único na linha do tempo. 
(isso pode ser melhorado... pq o primeiro dado pode ser um outlier e o segundo se encaixar melhor, mas para esse caso vamos manter assim, a base esta bem sobria)

### 4.4.3 Saneamento e Outliers
Detecção de anormalidades (Z-Score): Utilizou-se a lógica de Z-Score móvel (com janela de 12 meses) para identificar saltos absurdos ($|Z| > 3$)Z-Score móvel (com janela de 12 meses) para identificar saltos absurdos ($|Z| > 3$)

### 4.4.4 Padronização
Diferente de séries de volume bruto, a PIM-PF utiliza o Número-índice de base fixa (2012=100). Esta é uma forma de padronização realizada pelo próprio IBGE que permite a comparação direta entre diferentes segmentos industriais e regiões, utilizando a média de 2012 como ponto de equilíbrio (100).

Adicionalmente, para fins de modelagem estatística, os dados foram submetidos a transformações de logaritmo e diferenciação, visando estabilizar a variância e garantir a estacionariedade da série, conforme exigido pelos modelos de classe SARIMA.Diferente de séries de volume bruto, a PIM-PF utiliza o Número-índice de base fixa (2012=100). Esta é uma forma de padronização realizada pelo próprio IBGE que permite a comparação direta entre diferentes segmentos industriais e regiões, utilizando a média de 2012 como ponto de equilíbrio (100).

Adicionalmente, para fins de modelagem estatística, os dados foram submetidos a transformações de logaritmo e diferenciação, visando estabilizar a variância e garantir a estacionariedade da série, conforme exigido pelos modelos de classe SARIMA.

## 4.5 EDA
O processo de investigação analítica segue o seguinte fluxo de trabalho:Pré-processamento: Conversão dos dados do formato Wide para Long e tratamento da tipagem temporal (datetime).Análise de Estacionariedade: Aplicação do teste de raiz unitária (Augmented Dickey-Fuller) para verificar se a série exige diferenciação.Decomposição Sazonal: Separação estatística da Tendência ($T_t$) e Sazonalidade ($S_t$), validando a escolha da periodicidade mensal para capturar os ciclos produtivos anuais.Levantamento de Técnicas: Definição de modelos de suavização exponencial (Holt-Winters) e modelos autorregressivos para a fase de predição.
### 4.5.1 Graficos
### 4.5.2 Decomposição STL
### 4.5.1 EVM e EVA




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

COTTA, Paulo. 
Introdução ao ARIMA e SARIMA: modelos de séries temporais. Medium, 2023. 
Disponível em: https://medium.com/@paulovpcotta/introdu%C3%A7%C3%A3o-ao-arima-e-sarima-modelos-de-s%C3%A9ries-temporais-51992ae5abfd. 
Acesso em: 24 abr. 2026.

DATA SCIENCE ACADEMY. 
Análise e Modelagem de Séries Temporais: Técnicas Estatísticas, IA e Suas Aplicações. Blog DSA, 2023. 
Disponível em: https://blog.dsacademy.com.br/analise-e-modelagem-de-series-temporais-tecnicas-estatisticas-ia-e-suas-aplicacoes/. 
Acesso em: 24 abr. 2026.

DUTT, Rohan. 
10 Hybrid Forecasting Architectures: Blending Deep Learning with Time Series Models. Medium, 2023. 
Disponível em: https://medium.com/@Rohan_Dutt/10-hybrid-forecasting-architectures-blending-deep-learning-with-time-series-models-252c685601e1. 
Acesso em: 24 abr. 2026.

GEEKSFORGEEKS. 
SARIMA (Seasonal Autoregressive Integrated Moving Average). GeeksforGeeks, 2024. 
Disponível em: https://www.geeksforgeeks.org/machine-learning/sarima-seasonal-autoregressive-integrated-moving-average/. Acesso em: 25 abr. 2026.

IBGE. PIM-PF - Pesquisa Industrial Mensal - Produção Física: Tabela 8159. Rio de Janeiro: IBGE, 2022. Disponível em: https://sidra.ibge.gov.br/tabela/8159. Acesso em: 25 abr. 2026.

LIU, Yong; LIU, Chen; et al. 
Koopa: Forecasting Non-stationary Time Series with Disentangled Koopman Dynamics. 
Medium, 2023. Disponível em: https://medium.com/@kdk199604/koopa-forecasting-non-stationary-time-series-with-disentangled-koopman-dynamics-f3348aa5d4be. 
Acesso em: 26 abr. 2026.
