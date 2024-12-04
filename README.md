# projeto-avd-2024.2
Projeto no formato de dashboard desenvolvido para analisar eventos terroristas globais de 1970 a 2021, baseado no Banco de Dados Global sobre Terrorismo (GTD - Global Terrorism Database), da Universidade de Maryland, fornecendo insights sobre padrões temporais, impacto geográfico e tipos de ataques.

Escolha dos Elementos Visuais 
1. Mapa de Bolha 
o Objetivo: Explorar o impacto geográfico dos ataques terroristas. 
o Por quê? Este visual permite identificar rapidamente os países mais afetados, 
destacando o número de mortes por ataque em cada região. 
o Configuração: 
▪ Eixo de Localização: country_txt (País). 
▪ Tamanho: nkill (Número de Mortes). 
2. Gráfico de Linha 
o Objetivo: Analisar a evolução do número de ataques e mortes ao longo do tempo. 
o Por quê? Exibe padrões temporais, como picos em anos específicos, ajudando a 
entender períodos de maior intensidade. 
o Configuração: 
▪ Eixo X: iyear (Ano). 
▪ Eixo Y: nkill (Número de Mortes). 
3. Gráfico de Barras (Distribuição por Tipo de Ataque): 
o Objetivo: Comparar a frequência de mortes por diferentes tipos de ataques. 
o Por quê? Ajuda a identificar quais ataques causaram mais impacto em termos de 
vítimas. 
o Configuração: 
▪ Eixo Y: attacktype1_txt (Tipo de Ataque). 
▪ Valores: nkill (Número de Mortes). 
Operações OLAP 
1. Drill-Down e Drill-Up: 
o Uso: No gráfico de linha, foi implementada uma hierarquia de dados (Ano → Mês → 
Dia), permitindo que o usuário amplie ou reduza o nível de detalhamento temporal. 
o Benefício: Detalhamento de eventos em períodos específicos, como analisar ataques 
em um mês específico. 
2. Slice and Dice: 
o Uso: Filtros para country_txt (País) e attacktype1_txt (Tipo de Ataque) foram 
adicionados. 
o Benefício: Exploração segmentada dos dados, permitindo análises personalizadas, 
como visualizar apenas ataques em um país específico. 
3. Ranking: 
o Uso: No gráfico de barras, foi configurada uma classificação para exibir os 5 maiores 
tipos de ataque em termos de mortes. 
o Benefício: Destaque para os ataques mais letais, facilitando a priorização da análise. 
Design do Dashboard 
1. Minimalismo: 
o Por quê? Um design claro e simples reduz distrações e facilita a interpretação rápida 
dos dados. 
o Implementação: 
▪ Esquema de cores consistente e neutro. 
▪ Elementos visuais espaçados para evitar sobrecarga de informações. 
▪ Rótulos e títulos explicativos. 
2. Interatividade: 
o Adicionados filtros dinâmicos para que o usuário possa explorar diferentes 
perspectivas dos dados sem sair da interface principal. 
Conclusão 
Este dashboard atende aos objetivos de análise, permitindo: 
• Identificar padrões temporais e geográficos de ataques. 
• Explorar interativamente os dados com filtros e drill-down. 
• Destacar ataques mais letais com ranking. 
O uso combinado de gráficos e operações OLAP proporciona uma experiência analítica rica, clara 
e focada, promovendo insights significativos sobre a complexidade dos eventos terroristas globais.
