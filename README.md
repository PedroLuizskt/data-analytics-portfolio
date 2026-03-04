<div align="center">
  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=F2C811&height=120&section=header"/>
  
  <a href="#">
    <img src="https://readme-typing-svg.herokuapp.com/?color=F2C811&size=35&center=true&vCenter=true&width=1000&lines=Business+Analytics;Power+BI+%26+DAX+Avançado;Data+Science+Aplicada&duration=4000&pause=1000" alt="Typing SVG" />
  </a>
</div>

<div align="center">

  [![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
  [![Data Science](https://img.shields.io/badge/Data_Science-005B96?style=for-the-badge&logo=databricks&logoColor=white)](#)
  [![Estatística Aplicada](https://img.shields.io/badge/Estatística-4B0082?style=for-the-badge&logo=spdx&logoColor=white)](#)

</div>

---

## 📊 Sobre o Repositório: De Dados a Decisões Estratégicas



Bem-vindo ao meu portfólio de **Data Science e Business Analytics**. 

Este repositório documenta minha jornada de evolução analítica, consolidando conhecimentos adquiridos!

O objetivo principal deste espaço não é apenas demonstrar proficiência técnica em ferramentas como Power BI, Power Query e DAX, mas sim comprovar a capacidade de traduzir dados brutos em **insights acionáveis** e orientados à resolução de problemas reais de negócio. Cada projeto aqui estruturado segue a premissa de que a tecnologia é apenas o meio; o fim é a tomada de decisão inteligente.

---

## 📂 Portfólio de Projetos e Laboratórios

Abaixo está o índice das análises desenvolvidas. Clique nos links para acessar os arquivos originais.

### 🧪 Lab 01: Análise Exploratória de Vendas Globais
**Arquivos:** [`Dashboard (.pbix)`](./Lab01/Lab1.pbix) | [`Visualização do Dashboard (.png)`](./Lab01/Lab1.png)

Este laboratório introdutório foca na construção de um panorama executivo (Overview) para uma empresa multinacional fictícia, com o objetivo de responder a perguntas de negócios essenciais sobre faturamento e distribuição geográfica.

**1. Contexto de Negócio**
Diretores comerciais precisam de respostas rápidas sobre a saúde financeira da empresa. O foco aqui é a **Análise Descritiva**: entender o que aconteceu nas vendas globais, identificando quais categorias de produtos impulsionam a receita e como as prioridades de entrega impactam o volume de vendas por região.

**2. Conceito Teórico Essencial**
* **Análise Exploratória de Dados (EDA):** Utilização de métricas de agregação (soma e média) para resumir grandes volumes de dados.
* **Geolocalização Analítica:** Mapeamento espacial para facilitar a identificação visual de clusters de alta rentabilidade. 

**3. Aplicação Prática no Power BI**
* **Métricas de Faturamento:** Criação de *Cards* para visualizar o Valor Total Vendido.
* **Distribuição Categórica:** Gráficos de barras para comparar o volume de vendas entre categorias de produtos de forma decrescente (Facilitando a leitura do Princípio de Pareto).
* **Matriz de Prioridade:** Tabelas/Matrizes cruzando as vendas por País com a variável categórica de Prioridade de Entrega.
* **Média Estatística Simples:** Cálculo da média de descontos aplicados, segmentada por subcategoria.
* **Visualização Geoespacial:** Uso do visual de Mapa para plotar os países de acordo com a magnitude da média do valor de venda.
* **Interatividade (Filtros contextuais):** Implementação de *Slicers* (Segmentadores de dados) permitindo ao usuário final fatiar o relatório por Ano, Segmento e País.

**4. Insight Analítico Gerado**
A estrutura construída permite que o tomador de decisão identifique rapidamente gargalos geográficos de vendas, avalie a política de descontos por subcategoria e ajuste estratégias de estoque com base na demanda categórica e prioridades de envio.

<div align="center">
  <img src="./Lab01/Lab1.png" alt="Demonstração Lab 01" width="80%">
</div>

---

### 🧪 Lab 02: Modelagem, Limpeza de Dados e Inteligência com DAX
**Arquivos:** [`Dashboard (.pbix)`](./Lab02/Lab2.pbix) | [`Visualização do Dashboard (.png)`](./Lab02/Lab2.png)

Neste laboratório, o foco avança para a engenharia analítica e a lógica de negócios. Além de responder a perguntas gerenciais, o projeto demonstra o tratamento prévio dos dados, a estruturação de relacionamentos (cardinalidade) e a introdução à linguagem DAX para criação de métricas financeiras customizadas.



**1. Contexto de Negócio**
A diretoria precisa ir além do faturamento bruto. O foco agora é entender a **Lucratividade** e a **Eficiência Logística**. O negócio estabeleceu uma meta clara (Valor médio de venda de 350) e precisa monitorar se as operações de envio estão corroendo as margens de lucro ao longo do tempo.

**2. Conceito Teórico Essencial**
* **ETL e Qualidade de Dados:** O uso do Power Query para higienização dos dados antes da modelagem garante que a análise não seja distorcida por dados sujos ou nulos.
* **Modelagem Relacional (Cardinalidade):** Estruturação correta de como as tabelas se conversam (ex: 1 para Muitos) para que os filtros funcionem perfeitamente.
* **Métricas vs. Colunas Calculadas (DAX):** Entendimento de quando calcular valores linha a linha (como o Lucro por transação) e quando usar agregações dinâmicas (como a Margem de Lucro geral).

**3. Aplicação Prática no Power BI**
* **Transformação de Dados:** Uso de recursos de limpeza do Power BI para padronizar as fontes de dados.
* **Visualização de Fluxo (Gráfico de Cascata):** Implementado para entender a composição do Total de Vendas quebrado por Modo de Envio, mostrando como cada modalidade soma ao total.
* **Distribuição Proporcional (Treemap):** Utilizado para mapear de forma hierárquica e visual quais Mercados representam o maior Custo Médio de Envio.
* **Monitoramento de Metas (Visual de KPI):** Criação de um indicador para comparar o Valor Médio de Vendas mensal contra o *target* fixo de 350 (permitindo auditar rapidamente meses específicos, como Abril/2014).
* **Engenharia de Features com DAX:** * Criação da medida de Lucro (`Lucro = Valor de Venda - Custo de Envio`) para descobrir a Categoria de Produto mais rentável.
  * Criação da medida de Margem (`Margem de Lucro = DIVIDE(Lucro, Valor de Venda)`) para analisar a proporção do lucro sobre a receita.
* **Análise Temporal:** Gráfico de linhas para monitorar a flutuação da Margem de Lucro ao longo do eixo de tempo, identificando tendências ou sazonalidades.

**4. Insight Analítico Gerado**
A análise revela não apenas o faturamento, mas a saúde real da operação. Ao cruzar o custo de envio com a margem de lucro temporal e aplicar o KPI contra a meta de 350, o negócio ganha insumos para renegociar contratos logísticos em mercados ineficientes e focar esforços de vendas nas categorias que de fato trazem rentabilidade (lucro real), e não apenas volume.

<div align="center">
  <img src="./Lab02/Lab2.png" alt="Demonstração Lab 02" width="80%">
</div>

---

### 🧪 Lab 03: Financial Analytics e Estruturação de Balanço Patrimonial
**Arquivos:** [`Dashboard (.pbix)`](./Lab03/Lab3.pbix) | [`Visualização do Dashboard (.png)`](./Lab03/Lab3.png)

Este laboratório marca a transição para a análise de dados financeiros. O objetivo central é demonstrar como transpor demonstrações contábeis estáticas e tradicionais para um ambiente interativo, explorando as capacidades avançadas de hierarquia e formatação do visual de Matriz no Power BI.



**1. Contexto de Negócio**
Para a diretoria financeira (CFO) e analistas de controladoria, o Balanço Patrimonial é a fotografia da saúde da empresa. O grande desafio das empresas tradicionais é sair do "Excel estático" e ter uma visão dinâmica de seus Ativos (o que a empresa tem), Passivos (o que a empresa deve) e Patrimônio Líquido, permitindo navegar do macro (visão consolidada) para o micro (contas contábeis específicas) em poucos cliques.

**2. Conceito Teórico Essencial**
* **Engenharia de Dados Financeiros:** Estruturação de dados em formato de plano de contas (hierarquias de níveis contábeis).
* **Equação Fundamental da Contabilidade:** Garantir a integridade lógica onde $Ativos = Passivos + Patrimônio Líquido$ na modelagem e exibição dos dados.
* **Drill-down e Drill-up Analítico:** O conceito de navegação em profundidade de dados hierárquicos para investigação de anomalias financeiras.

**3. Aplicação Prática no Power BI**
* **Domínio do Visual de Matriz:** Configuração avançada da Matriz para suportar estruturas financeiras complexas.
* **Layout de Níveis (Stepped Layout):** Ajuste de formatação para simular a identação clássica de relatórios contábeis, tornando a leitura intuitiva para profissionais de finanças.
* **Controle de Subtotais e Totais:** Manipulação das configurações do visual para exibir subtotais apenas nos níveis hierárquicos corretos (ex: Total do Ativo Circulante, Total do Passivo Não Circulante).
* **Navegação Hierárquica:** Implementação de recursos de expansão e recolhimento (Drill-down/Drill-up) permitindo ao usuário investigar a composição de contas específicas sem perder o contexto global.
* **Formatação Condicional e Estilização:** Aplicação de regras de design e UX (User Experience) voltadas para relatórios executivos, garantindo clareza e sobriedade.

**4. Insight Analítico Gerado**
A entrega deste dashboard transforma a rotina de auditoria e análise financeira. O tomador de decisão passa a ter uma ferramenta interativa que não apenas consolida a posição patrimonial da empresa em tempo real, mas também permite identificar rapidamente gargalos de liquidez ou alavancagem excessiva ao descer o nível de granularidade das contas com um simples clique.

<div align="center">
  <img src="./Lab03/Lab3.png" alt="Demonstração Lab 03" width="80%">
</div>

---

### 🚀 Projeto 01: Marketing Analytics e Comportamento do Consumidor
**Arquivos:** [`Dashboard (.pbix)`](./Projeto01/Projeto01.pbix)

Este é o primeiro projeto completo e estruturado do portfólio. Ele transcende a criação de gráficos isolados e apresenta uma solução robusta de **Business Intelligence aplicada ao Marketing**, composta por 4 painéis integrados. O objetivo é fornecer uma visão 360º da jornada do cliente, desde o seu perfil demográfico até a sua resposta às campanhas publicitárias.

**1. Contexto de Negócio**
O Diretor de Marketing (CMO) de uma empresa precisa otimizar o orçamento (Budget) das campanhas promocionais. Atirar para todos os lados custa caro e traz baixo retorno. O problema de negócio aqui é claro: **Quem é o nosso cliente ideal, o que ele compra e quais campanhas realmente funcionam?** Precisamos mapear o perfil do consumidor e cruzar isso com o volume de vendas e a aceitação das campanhas globais.

**2. Conceito Teórico Essencial**
* **Customer Analytics & Profiling:** Segmentação de clientes com base em variáveis demográficas (idade, renda, estado civil) e comportamentais (frequência de compra, recência).
* **Métricas de Efetividade:** Avaliação matemática de campanhas. Em Data Science aplicada ao marketing, frequentemente modelamos taxas de sucesso, como a Taxa de Conversão:
  $$Taxa\ de\ Convers\tilde{a}o = \frac{Total\ de\ Clientes\ que\ Compraram}{Total\ de\ Clientes\ Impactados\ pela\ Campanha}$$
* **Data Cleansing Avançado:** Identificação e tratamento de anomalias na base de dados (outliers, valores ausentes ou inconsistentes) que poderiam enviesar a análise das campanhas.

**3. Aplicação Prática no Power BI**
* **ETL e Correção de Dados:** Uso intensivo do Power Query para higienizar a base customizada, garantindo que as métricas reflitam a realidade.
* **Storytelling em 4 Visões (Páginas):**
  * **Visão do Cliente:** Foco em demografia (Renda, Escolaridade, Estado Civil).
  * **Visão do Comportamento de Compra:** Foco em transações (Ticket Médio, Volume por Categoria de Produto).
  * **Visão de Performance das Campanhas:** Foco em ROI e aceitação (Qual campanha teve maior adesão?).
  * **Visão de Padrões no PDV (País):** Foco geoespacial (Como os hábitos mudam de acordo com a região?).
* **Modelagem e DAX:** Criação de mais de 10 elementos visuais complexos, sustentados por medidas DAX customizadas para cruzar o perfil do cliente com o resultado financeiro.
* **UX/UI Design:** Aplicação de formatações avançadas, paleta de cores coesa e navegação fluida entre as 4 páginas do relatório para melhorar a experiência do usuário final.

**4. Insight Analítico Gerado**
A estrutura deste projeto permite à equipe de Marketing abandonar o "achismo". Ao cruzar a *Visão do Cliente* com a *Visão de Campanhas*, o negócio consegue identificar nichos hiper-específicos (ex: "Clientes casados, com alta renda, respondem 40% melhor à Campanha X no país Y"). Isso possibilita a criação de campanhas direcionadas, reduzindo o Custo de Aquisição de Clientes (CAC) e maximizando o retorno sobre o investimento.

#### 📸 Galeria do Projeto

<table align="center">
  <tr>
    <td align="center"><strong>Visão do Cliente</strong><br><img src="./Projeto01/1.png" alt="Visão do Cliente" width="100%"></td>
    <td align="center"><strong>Visão do Comportamento</strong><br><img src="./Projeto01/2.png" alt="Visão do Comportamento de Compra" width="100%"></td>
  </tr>
  <tr>
    <td align="center"><strong>Visão das Campanhas</strong><br><img src="./Projeto01/3.png" alt="Visão da Performance das Campanhas" width="100%"></td>
    <td align="center"><strong>Visão do PDV (País)</strong><br><img src="./Projeto01/4.png" alt="Visão dos Padrões de Compra no PDV" width="100%"></td>
  </tr>
</table>

---

### 🚀 Projeto 02: Inteligência Comercial e Augmented Analytics (Análise Aumentada)
**Arquivos:** [`Dashboard (.pbix)`](./Projeto02/Projeto02.pbix)

Neste projeto, elevamos a maturidade analítica saindo da análise puramente descritiva (o que aconteceu) para a **Análise Diagnóstica** (por que aconteceu). Utilizando dados comerciais de uma empresa fictícia, este painel aplica recursos de Inteligência Artificial integrados ao Power BI e foca na experiência do usuário (UX) através de navegação por menus.

**1. Contexto de Negócio**
O Diretor de Vendas (CSO - *Chief Sales Officer*) não tem tempo para procurar os motivos de uma queda ou alta no faturamento. Ele precisa que o painel lhe diga imediatamente quais fatores impulsionam os resultados e como o ranking de produtos flutua ao longo dos trimestres. O objetivo é responder: **O que influencia nosso sucesso e qual a narrativa por trás dos números?**

**2. Conceito Teórico Essencial**
* **Machine Learning & Probabilidade Condicional:** O visual de "Principais Influenciadores" roda modelos estatísticos (como Regressão Logística e Árvores de Decisão) no *backend* para calcular a probabilidade de um evento ocorrer dado um fator específico: $P(\text{Aumento nas Vendas} \mid \text{Fator}_X)$.
* **Natural Language Processing (NLP):** Geração de texto dinâmico a partir de dados estruturados para criar resumos executivos automáticos.
* **Análise de Volatilidade de Rankings:** Avaliação de como a posição competitiva de categorias ou produtos muda no eixo temporal.

**3. Aplicação Prática no Power BI**
* **UX/UI e Navegação Estruturada:** Criação de uma página de "Índice" (Menu principal) com o uso de *Bookmarks* (Indicadores) e Botões, permitindo uma navegação fluida estilo aplicativo (App-like experience) entre as visões do relatório.
* **Inteligência Artificial (Principais Influenciadores):** Implementação do visual de IA para descobrir automaticamente quais segmentos, regiões ou categorias puxam a métrica de vendas para cima ou para baixo.
* **Geração de Texto (Narrativa Inteligente):** Uso do visual de Narrativa para criar uma caixa de texto que se reescreve sozinha baseada nos filtros aplicados, destacando anomalias, picos e quedas.
* **Gráfico de Faixas (Ribbon Chart):** Utilizado não apenas para ver o volume financeiro, mas para visualizar a transição e a quebra de posições (Rankings) entre categorias de produtos ao longo dos meses.

**4. Insight Analítico Gerado**
Este projeto entrega um verdadeiro "assistente de vendas" ao gestor. Ao invés de o usuário ter que deduzir tendências visualmente, os algoritmos do painel apontam os direcionadores de lucro. Se a região "Sul" de repente se torna o principal influenciador de alta, a equipe comercial pode imediatamente replicar as estratégias dessa região para as demais. A navegação por botões garante que até o usuário menos técnico consiga extrair esse valor sem frustração.

#### 📸 Galeria do Projeto

<table align="center">
  <tr>
    <td align="center"><strong>Menu de Navegação (Índice)</strong><br><img src="./Projeto02/1.png" alt="Índice do Dashboard" width="100%"></td>
    <td align="center"><strong>Visão Geral de Vendas</strong><br><img src="./Projeto02/2.png" alt="Visão Comercial 1" width="100%"></td>
  </tr>
  <tr>
    <td align="center"><strong>Gráfico de Faixas (Rankings Temporais)</strong><br><img src="./Projeto02/3.png" alt="Gráfico de Faixas" width="100%"></td>
    <td align="center"><strong>Principais Influenciadores (Machine Learning)</strong><br><img src="./Projeto02/4.png" alt="Principais Influenciadores" width="100%"></td>
  </tr>
  <tr>
    <td colspan="2" align="center"><strong>Narrativa Inteligente (Geração de Linguagem Natural - NLP)</strong><br><img src="./Projeto02/5.png" alt="Narrativa Inteligente" width="60%"></td>
  </tr>
</table>

---

### 🧑‍💼 Projeto 03: People Analytics e Gestão Estratégica de Talentos
**Arquivos:** [`Dashboard (.pbix)`](./Projeto03/Projeto03.pbix) | [`Visualização do Dashboard (.png)`](./Projeto03/projeto03.png)

Neste projeto, o foco é a área de Recursos Humanos. O objetivo é transformar dados operacionais de funcionários em inteligência estratégica, aplicando os conceitos de **People Analytics**. O projeto também destaca a maturidade no desenvolvimento em Power BI através da organização de arquitetura (Tabela de Medidas) e lógica de programação (Colunas Condicionais).



**1. Contexto de Negócio**
O Diretor de RH (CHRO) precisa de um panorama exato da força de trabalho atual para tomar decisões sobre políticas de diversidade, orçamento de folha de pagamento e planos de carreira. A empresa precisa mapear o nível de envolvimento das equipes, a disponibilidade para horas extras (impacto direto em custos operacionais e *Burnout*) e, principalmente, prever o orçamento para o próximo ciclo de promoções baseado em regras de negócio claras e justas.

**2. Conceito Teórico Essencial**
* **People Analytics & Demografia Organizacional:** Estudo do comportamento, experiência e distribuição demográfica da força de trabalho para otimizar a gestão de talentos.
* **Feature Engineering (Transformação de Variáveis Contínuas em Categóricas):** O processo de pegar um número absoluto (ex: Anos desde a última promoção) e transformá-lo em uma classe de decisão (Elegível / Não Elegível). Em estatística e programação, representamos essa lógica condicional (*Step Function*) da seguinte forma:
  $$Promo\c{c}\tilde{a}o(x) = \begin{cases} \text{Considerar Promo\c{c}\tilde{a}o}, & \text{se } x \ge 5 \\ \text{N\tilde{a}o Considerar}, & \text{se } x < 5 \end{cases}$$
  *(Onde $x$ é o número de anos desde a última promoção).*

**3. Aplicação Prática no Power BI**
* **Arquitetura de Medidas (Measures Table):** Abandono da prática amadora de espalhar medidas pelas tabelas do modelo. Criação de uma tabela virtual dedicada exclusivamente para centralizar e organizar o código DAX, facilitando a manutenção do sistema.
* **Lógica Condicional no Power Query/DAX:** Implementação de regras de negócio customizadas para criar a flag de "Elegibilidade para Promoção" (variável calculada fora do dashboard visual, mas essencial para o *backend* analítico).
* **Métricas de Capital Humano (KPIs):** Cálculos de *Headcount* (Total de funcionários), Tempo Médio de Experiência (Senhoridade da equipe) e Média Salarial Mensal.
* **Análise de Diversidade e Engajamento:** Estruturação de visuais para analisar a proporção de gênero na empresa, o nível de envolvimento dos colaboradores (segmentado em Ruim, Baixo, Médio e Alto) e a distribuição da força de trabalho por funções específicas.

**4. Insight Analítico Gerado**
Com este painel, o RH deixa de ser reativo e passa a ser preditivo. Ao cruzar o nível de envolvimento com o tempo médio de experiência e a disponibilidade para horas extras, a gestão pode identificar potenciais talentos sobrecarregados (risco de *Turnover*). Além disso, o cálculo exato do percentual de funcionários elegíveis para promoção permite à diretoria financeira (CFO) provisionar o orçamento do próximo ano com base em dados reais, e não em estimativas.

#### 📸 Visão Geral do Painel de RH

<div align="center">
  <img src="./Projeto03/projeto03.png" alt="Dashboard de People Analytics" width="85%">
</div>

---
