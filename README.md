# Avaliação de Teste A/B e Funil de Conversão

## Objetivo do Projeto
Avaliar o desempenho de um teste A/B associado a um novo sistema de recomendação e analisar o funil de eventos dos utilizadores para verificar se o experimento atingiu os ganhos esperados de conversão nas etapas do funil e sustentar uma decisão baseada em dados.

## Ferramentas e Bibliotecas
* **Linguagem:** Python
* **Manipulação e Análise de Dados:** Pandas, NumPy, SciPy
* **Visualização de Dados:** Matplotlib, Seaborn, Plotly

## Estrutura dos Dados
O estudo baseia-se nos conjuntos de dados do projeto `recommender_system_test` da TripleTen (ficheiros originais omitidos do repositório por direitos de utilização, com todos os cálculos, tabelas e gráficos preservados no notebook):

* **Dados de marketing e participantes:** identificadores de utilizador, grupo do teste (`A` ou `B`) e canal/região de origem.
* **Registo de eventos:** carimbo temporal (`event_dt`), funil login - product_page - product_cart - purchase e `user_id`.

## Metodologia
1. **Preparação e Limpeza dos Dados:** Verificação de valores ausentes, tipos de dados, duplicações e alinhamento da janela temporal do experimento e das regras de participação.
2. **Análise Exploratória e Funil de Conversão:** Contagem de eventos e utilizadores únicos por etapa do funil, cálculo das taxas de conversão entre etapas e comparação do comportamento entre os grupos.
3. **Avaliação do Teste A/B e Testes de Hipóteses:** Verificação de sobreposição de utilizadores entre grupos, análise da distribuição diária de eventos e aplicação de testes estatísticos de proporções (teste Z) para validar diferenças estatisticamente significativas.

## Principais Conclusões e Recomendações
* Síntese das diferenças observadas entre os grupos A e B ao longo do funil e avaliação se os resultados justificam o lançamento ou ajustes no experimento.
* Recomendações práticas para o acompanhamento de métricas e otimização da conversão.

