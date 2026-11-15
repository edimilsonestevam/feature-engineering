# Feature Engineering

O dataset disponibilizado para a sua equipe possui informações apenas de solicitações de cartão de crédito que foram aprovadas, ou seja, todos os registros são de clientes da empresa. Os clientes são marcados como maus pagadores ("bad" - última coluna "**ROTULO_ALVO_MAU=1**") se houver **atraso de maior de 60 dias** no pagamento da fatura durante o primeiro ano após a contratação.

A melhoria do dataset deverá ser feita com base nas técnicas fundamentais de Feature Engineering como **imputação de dados**, **normalização**, **codificação de variáveis categóricas**, **seleção de características** etc.

A avaliação das melhorias do dataset deverá ser feita através da análise de performance obtida com o treinamento de um classificador escolhido pelo grupo (**Regressão Logística**, **Random Forest** etc) para predição de bons e maus pagadores. Para garantir que não haja interferência de outros fatores na análise, alguns cuidados deverão ser tomados:

* Atenção para que tenhamos efeito comparativo entre os modelos (quais parâmetros devem ser preservados e quais podem mudar);
* A divisão do dataset entre treino e teste deverá ser feito sempre com a mesma **randoom_seed** para garantir que flutuações geradas por mudanças na composição do dataset não afetem na avaliação.

---

**Entregáveis**

Ao término do projeto a equipe deverá fazer as seguintes entregas:

Arquivo PowerPoint com análises e resultados:

A apresentação deverá conter não apenas o **resultado final obtido** e uma **explicação detalhada das decisões tomadas** para atingir o resultado alcançado. Em particular, alguns pontos são extremamente importantes:

* Detalhamento de todas as **Técnicas de Feture Engineering** aplicadas no dataset com justificativas das decisões tomadas;
* Resultados intermediário que a equipe julgar importante apresentar para demonstrar a **evolução de qualidade** do dataset;
* Análise de acurácia matriz de confusão e demais métricas de classificadores dos resultados apresentados.

---

**Jupyter Notebook**

O notebook deverá estar bem organizado com seções claras e textos que facilitem a compreensãoi da análise e decisões tomadas e que permita a obtenção do resultado final a partir do dataset disponibilizado.

**Importante:** parte significativa da avaliação do resultado será feita com a execução do notebook. Desta forma é importante que todas as células executem corretamente e que os resultados sejam integralmente reprodutíveis.

---

**DATASET**

Ref.:

```Jupyter
df = pd.read_csv("https://raw.githubusercontent.com/diogenesjusto/FIAP/refs/heads/master/dados/credit_features_formatado.
csv")
```
