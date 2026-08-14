# 📊 Análise de Funil de Conversão e Experimento A/A/B

## 📌 Sobre o projeto

Este projeto analisa o comportamento dos usuários em um aplicativo de uma startup de produtos alimentícios, utilizando dados de eventos registrados durante a interação com a plataforma.

O objetivo foi compreender a jornada dos usuários dentro do aplicativo, identificar pontos de perda no funil de compra e avaliar se uma alteração no design da interface — especificamente, a mudança das fontes — teria impacto significativo no comportamento e na conversão dos usuários.

🎯 Objetivos

- Analisar o comportamento dos usuários dentro do aplicativo;
- Identificar as principais etapas da jornada de compra;
- Avaliar a conversão entre as etapas do funil;
- Identificar possíveis pontos de perda de usuários;
- Verificar a qualidade e consistência dos dados;
- Validar a divisão dos usuários entre os grupos de experimento;
- Avaliar, por meio de testes estatísticos, o impacto da mudança das fontes no comportamento dos usuários.

🛠️ Ferramentas e tecnologias
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook

🔎 Etapas da análise
1. Preparação dos dados

Inicialmente, foram realizadas análises de estrutura e qualidade dos dados, incluindo:

- Identificação dos tipos de dados;
- Padronização dos nomes das colunas;
- Verificação de valores ausentes;
- Identificação e remoção de registros duplicados;
- Conversão dos timestamps para formato de data e hora;
- Análise do período coberto pelos registros.

2. Análise do comportamento dos usuários

Após a preparação dos dados, foram analisados:

- Número total de eventos;
- Quantidade de usuários;
- Média de eventos por usuário;
- Distribuição dos eventos;
- Período de cobertura dos dados;
- Distribuição temporal dos registros.

3. Análise do funil de conversão

A jornada dos usuários foi analisada a partir dos eventos registrados no aplicativo, permitindo acompanhar a progressão entre diferentes etapas do processo de compra.

4. Experimento A/A/B

Na etapa experimental, os usuários foram divididos em três grupos, sendo 246, 247 e 248.

Primeiramente, foi realizado um teste A/A entre os grupos 246 e 247 para verificar se a divisão dos usuários apresentava comportamento semelhante.

Em seguida, o grupo experimental (248) foi comparado individualmente com cada grupo de controle e também com os dois grupos de controle combinados.

Os testes estatísticos foram utilizados para verificar se a alteração das fontes produziu diferenças estatisticamente significativas no comportamento dos usuários. Também foi aplicada a correção de Bonferroni, considerando o efeito das comparações múltiplas e reduzindo o risco de falsos positivos.

📈 Principais resultados
- Foram analisados 244.126 registros inicialmente;
- 413 registros duplicados foram identificados e removidos;
- A base final utilizada na análise possui 243.713 eventos;
- Foram identificados 7.551 usuários;
- A média foi de aproximadamente 32,28 eventos por usuário;
- A conversão total do funil foi de 47,7%;
- O teste A/A foi utilizado para validar a consistência entre os grupos de controle;
- O grupo experimental foi comparado com os grupos de controle individualmente e combinados;
- Foi aplicada a correção de Bonferroni, com nível de significância ajustado para 0,0025.

## 📓 Notebook

A análise completa pode ser consultada no notebook:

[👉 Acessar o notebook do projeto](analise-funil-conversao-experimento-aa-b.ipynb)
