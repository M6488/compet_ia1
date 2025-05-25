- Justificativa do database que escolhi.

Escolhi a banknote por ser bastante usada em projetos desse tipo, ela permite construir modelos de aprendizagem de máquina.
Em si o banknote foi criado para identificar notas bancárias e definir se elas são verdadeiras ou falas com base em apenas 4 variáveis que são estraídas de imagens digitalizadas.
Como são só 4 variáveis fica até fácil de trabalhar com esse database.
Fiz um pré processamento bem básico, pois nesse dataframe não tinha nenhum dado faltante. Coloquei o desvio padrão para 1 e separei o data frame em 2 tirando
a coluna class que é o valor que estou tentando prever com o código. Nesse caso 1 significa que as cédulas são verdadeiras e 0 que são falsas
treinei dois modelos que peguei do scikit-learn , alimentei com os dados da coluna class. O print na parte final mostra o modelo que mais conseguiu prever de forma acertiva (melhor desempenho no teste).

Consegui fazer os testes 30 vezes e determinar qual modelo foi mais eficiente, depois usei ele com o gradio.
