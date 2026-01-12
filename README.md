# Análise de Desempenho de Campanha de Marketing
## 📝 Introdução
O mercado de vendas tem se tornado cada vez mais **competitivo, dinâmico e orientado ao comportamento do consumidor**. Empresas atuam em múltiplos canais — como lojas físicas, e-commerce e catálogos — e enfrentam o desafio de **integrar dados, entender a jornada do cliente e maximizar resultados em um cenário de margens pressionadas.**
Entre os principais desafios estão a **fragmentação das informações, a dificuldade em medir a efetividade das campanhas, a otimização do investimento em marketing** e a necessidade de responder rapidamente às mudanças do mercado e às novas expectativas dos consumidores.
Nesse contexto, a **análise de dados** torna-se um fator crítico para identificar **ofensores de performance**, como canais pouco eficientes, baixa taxa de conversão, custos elevados de aquisição e falta de visibilidade sobre indicadores-chave. Empresas que não utilizam dados de forma estratégica tendem a tomar decisões reativas, enquanto organizações orientadas por dados ganham **vantagem competitiva**, eficiência operacional e maior assertividade em suas decisões comerciais.

## 📊 Problema de Negócio

Diante de um mercado cada vez mais competitivo e multicanal, a empresa **NovaVibe** (empresa fictícia do setor de varejo) identificou a necessidade de avaliar de forma mais estruturada o desempenho de sua **campanha de marketing**, distribuída entre **loja física, e-commerce e catálogo**.
Embora a campanha estivesse ativa, a ausência de uma visão consolidada dos dados dificultava a compreensão sobre quais canais estavam gerando maior volume de vendas, quais apresentavam menor eficiência e onde os esforços de marketing poderiam ser otimizados. As decisões, até então, eram baseadas em percepções isoladas, sem o suporte de indicadores claros e comparáveis.

## 📈 Contexto

Nesse contexto, este case tem como objetivo realizar uma **análise exploratória e descritiva da campanha de marketing**, utilizando dados para **avaliar a performance por canal**, identificar **padrões de comportamento de compra** e gerar **insights que apoiem a tomada de decisão estratégica**. O foco da análise é transformar dados brutos em informações relevantes, permitindo uma visão clara dos resultados da campanha e apoiando ações de melhoria e otimização dos investimentos em marketing.

## 💾 Fonte dos Dados

A base de dados utilizada neste projeto foi obtida na plataforma **Kaggle** e é utilizada exclusivamente para fins educacionais, com o objetivo de demonstrar habilidades em Análise de Dados, visualização e geração de insights.

## 📌 Premissas da Análise
1. A campanha visa analisar o que ocorreu entre os dias 15 Janeiro de 2025 até 30 de Janeiro de 2025;
2. A variável Custo_Contato apresenta valor constante para todos os registros, o que inviabiliza análises comparativas de custo entre campanhas. Dessa forma, ela foi utilizada apenas como parâmetro fixo para o cálculo de métricas agregadas, como custo total e ROI;
3. A variável Receita_Campanha encontra-se no mesmo cenário do item 2;
   
## 🎯 Estratégia da Solução

O método **Fato-Dimensão** foi utilizado para desenvolver a análise de dados da campanha de Marketing.

### Passo 1: Resumir o contexto em uma pergunta aberta
Na **análise de dados**, uma **pergunta aberta** é aquela que **não pode ser respondida apenas com “sim”, “não” ou um valor único**. Ela exige **exploração, interpretação e análise**, permitindo descobrir padrões, causas e oportunidades. Para esse estudo foi definida a seguinte pergunta aberta: **"Como aumentar o resultado da próxima campanha de Marketing?"**

### Passo 2: Transformar perguntas abertas em perguntas fechadas
Em **análise de dados**, uma **pergunta fechada** é aquela que **possui respostas limitadas, diretas e objetivas**, geralmente podendo ser respondida com **“sim”/“não”, valores numéricos ou categorias específicas**. Para esse estudo foi definida a seguinte pergunta fechada: **"Quais são as características dos clientes que mais gastaram na campanha de Marketing?**

### Passo 3: Definição da coluna Fato
O **Fato** é uma **coluna de interesse** que representa o ponto focal da análise. Nesse caso, a coluna **"Gasto_Cliente"** representa o faturamento de cada cliente dentro de uma campanha e será o **objetivo** da nossa análise, dado que o problema do negócio envolve o **aumento do faturamento na próxima campanha de Marketing**.

### Passo 4: Identificação das Dimensões
Os campos foram estruturados em **dimensões compartilhadas**, permitindo uma análise mais detalhada do **fato principal**. Com base nessa estrutura, as seguintes dimensões foram estabelecidas::

**1. Cliente**
   - Salário
   - Idade
   - Faixa_Etária
   - Tempo Ativo Cliente
   - Estado Civil
   - Escolaridade
   - Filhos_Pequenos
   - Filhos_Adolescentes
   - Recência (Dias_Sem_Comprar)  
     
**2. Produto**
   - Gastos_Carne
   - Gastos_Vinho
   - Gastos_Doces
   - Gastos_Frutas
   - Gastos_Peixes
   - Gastos_Luxo
  
**3. Comportamento de Compra**
   - Gasto_Cliente
   - Compras_Online
   - Compras_Catálogo
   - Compras_Loja
   - Compras_Com_Desconto
   - Visitas_Web_Mensais
 
**4. Comportamento de MKT**
   - Reclamações
