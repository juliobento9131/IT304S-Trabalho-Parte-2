# Projeto `VIABILIDADE ECONÔMICA DE MIGRAÇÃO PARA O ACL DA UFFS – UNIVERSIDADE FEDERAL DA FRONTEIRA SUL`
# Project `ECONOMIC FEASIBILITY OF MIGRATION FOR ACL UFFS – UNIVERSIDADE FEDERAL DA FRONTEIRA SUL`

# Descrição Resumida do Projeto
~~~
<Análise da viabilidade econômica de migração para o mercado livre da UFFS – Universidade Federal da Fronteira Sul, contemplando 6 UCs – Unidades Consumidoras do Grupo A - com uma demanda contratada total de 1.022 kW, mediante o diagnóstico das informações oriundas das faturas de energia elétrica.>
~~~

# Abstract in English
~~~
<Analysis of the economic feasibility of migrating to the free market from UFFS - Federal University of the Southern Frontier, covering 6 UCs - Group A Consumer Units - with a total contracted demand of 1,022 kW, by diagnosing the information from the electricity bills.>
~~~

# Equipe
* `PEDRO PAULO CUNHA` `RA: 262248` 
* `JULIO CÉSAR BENTO` `RA: 262270`
* `DANILO FERNANDES PIRES` `RA: 210327`


# Vídeo do Projeto
`<coloque um link para o vídeo apresentado o projeto.>`

# Introdução e Motivação
~~~
<A migração para o mercado livre de contratação de energia elétrica ou Ambiente de Livre Contratação - ACL  pode representar uma grande oportunidade de economia com os gastos com esse insumo essencial para qualquer atividade. 
A Unicamp é um case de sucesso e referência nesse contexto e por meio da disciplina IT304S ofertada no segundo semestre de 2020 foram apresentadas, dentre vários assuntos correlatos, as premissas para migração para o ACL. 
Assim foi realizada a análise da Universidade Federal da Fronteira Sul - UFFS com o objetivo de concluir se é viável ou não a sua migração.
De forma resumida são apresentados a seguir a metodologia e considerações para a análise:
 - Digitação dos dados das faturas escaneadas em pdf para planilha salva no Google Drive;
 - Tratamentos estatísticos (eliminação de dados faltantes e tratamento de outliers) utilizando a plataforma Colab; 
 - Foi considerado o período de 2018 e 2019 como base para a sazonalidade de consumo e da demanda; 
 - Considerado 3% adicionais referentes às perdas da Rede Básica;
 - Com base na sazonalidade chegou-se a um valor de 0,35 MWmédios mensal (já somados os 3% de perdas);
 - Tarifas de energia elétrica vigentes na data de 18/01/2021 das distribuidoras locais RGE e COPEL;
 - Fonte incentivada com 50% de desconto na TUSD, verificados no dia 18/01/2021;
 - Foram considerados preços para um horizonte de 5 anos 2022 a 2026;
 - Não foram considerados os valores de consumo ponta, fora ponta e demanda referentes ao ano de 2020, dado o cenário de pandemia da COVID-19;
 - Foram considerados os impostos como PIS, COFINS e ICMS, dado que se trata de instituição de ensino e o ICMS é custo, logo foi considerado no estudo.
 Foi concluído que é viável e vantajosa a migração e o retorno médio do investimento se dará em um prazo muito curto (menor que 2 meses).
>
~~~

## Perguntas de Pesquisa
~~~
Vale a pena migrar para o Mercado Livre? Como consumidor livre ou especial?
R:Sim. Considerando as premissas aprensentadas como ponto de partida para a análise a migração é extremamente vantajosa.
Qual é a economia estimada?
R: Para primeiro ano a economia estimada foi de 23 a 29% a depender a bandeira tarifária considerada. Os demais anos analisados estão detalhados no arquivo (nome do arquivo) 
Qual é o preço da energia a partir de quando compensa a migração?
R: O Break Even Point ou preço de empate calculado foi de R$370,74 para a RGE e R$340,49 para a COPEL.
Qual a recomendação para uma contratação? (Características de contrato como volume, flexibilidade, modulação, sazonalização).
R: A recomendação é a contratação de 0,35MW médios na modalidade flex com variação de 15% acima ou abaixo.
~~~

## Objetivos do projeto
~~~
<Após a análise dos dados pode-se concluir que há viabilidade da migração (Parte II) e resultou na sugestão de melhorias contratuais nos valores de demanda contratada e em alguns casos do tratamento da potência reativa excedente (Parte I).>
~~~

# Recursos e Métodos

## Bases de Dados
Base de Dados | Endereço na Web | Resumo descritivo e uso
----- | ----- | -----
Base 1 | https://docs.google.com/spreadsheets/d/18-6rlREK_NcuQ1HUxrDe3B2V8_Uoz-Fx/edit?rtpof=true#gid=677347183 | `<Planilha preenchida com os dados das faturas>`
Base 2 | https://drive.google.com/drive/folders/1ZAIcggvx7E4GRHUXxhlhBKQJpz0bdlV8 | `<Faturas de energia elétrica escaneadas>`

## Ferramentas

Ferramenta | Endereço na Web | Resumo descritivo e uso
----- | ----- | -----
Ferramenta 1 | https://drive.google.com/drive/folders/1ZAIcggvx7E4GRHUXxhlhBKQJpz0bdlV8 | `<Drive da disciplina IT304S compartilhado com os alunos - Google Drive>`
Ferramenta 2 | https://colab.research.google.com/| `<Plataforma do Google Colab onde foram tratados os dados>`

# Metodologia

### Análise dos dados
~~~
# Definição de ciência de dados 
A ciência de dados pode ser definida como um conjunto de técnicas de analise de dados para obter e apresentar informações úteis para um usuario. 

# Metodologia
Uma metodologia muito utilizado para analisar dados é o chamado ``CRISP-DM", por suas siglas em inglês: Cross-Industry Standard Process for Data Mining. O CRISP-DM tem seis etapas que são:
 - Business Understanding:** Definição dos objetivos, declaração do problema, * * pergunta de interesse.
 - Data Understanding:** Utilização de nosso conhecimento para coletar os dados.
 - Data Preparation:** Manipulação de dados para a eliminação de outliers e dados faltantes.
 - Modeling:** Modelo ou abordagem utilizado para estudar o comportamento de nosso sistema a partir de nossos dados.
 - Evaluation:** Avaliação dos resultados obtidos, no contexto se são de ajuda para responder nossa pergunta de interesse.
 - Deployment:** Disponibilizar o análise de dados.

# Business Understanding
 - Definição dos objetivos:** O objetivo do presente notebook é apresentar as variaveis disponíveis no banco de dados UFFS.xlsx.
 - Declaração do problema:** O arquivo UFFS.xlsx, contém as informações disponíveis das planilhas elétricas da UFFS, precisamos de fazer um analize exploratorio dos dados para conhecer os dados disponíveis da UFFS.
 - Perguntas de Interesse:**
Há dados faltantes?

# Data Understanding
 - Coleta dos dados: Digitação dos dados das faturas em planilha eletrônica.

# Data Preparation
 - Eliminação de colunas com excesso de dados faltantes.
 - Tratamento das colunas com dados faltantes com a utilização de inerpolação quadrática e backward fill.
 - Tratamento das colunas para eliminação de outliers com o método Zscore.

# Modeling/Evaluation
 - Foi utilizado o modelo ARIMA para fazer uma fazer uma previsão dos dos ultimos doze meses. Foi observada uma discrepância na parte final do gráfico que já era esperada coniderando a drástica redução do consumo de energia por motivo da pendemia de COVID-19.
 
# Deployment
 - Os dados de cada UC foram disponibilizados em formato csv.
 
 Fonte: notebook gerado na aula do dia 14-12-2020. <https://github.com/byronacunia/IT304S.git>
~~~

### Avaliação da migração
~~~
A avaliação da migração foi feita comparando os gastos com energia elétrica considerando a forma convencional de fornecimento cativo e a com a opção de contratação no mercado livre. A cada mês foi computada a diferença e apresentada em forma de tabela e foi totalizada ao final do período de 5 anos (2022-2026).  
~~~

## Detalhamento do Projeto
~~~
Inicialmente, atualizou-se a planilha base com todas faturas disponibilizadas da UFFS – Universidade Federal da Fronteira Sul e, posteriormente foram feitos tratamentos estatísticos (preenchimento de dados faltantes e tratamento de outliers) utilizando a plataforma Colab. Em seguida, com a série de dados ajustada de cada UC, foi utilizado o período de 2018 e 2019 como base para a sazonalidade de consumo. A seguir são colocadas as premissas utilizadas para a migração para o ACL – Ambiente de Contração Livre da referida universidade:
 - A partir dos dados de medição de consumo ponta e fora ponta verificados nos históricos de consumo, chegou-se ao consumo total, onde foram acrescentados 3% adicionais referentes às perdas da rede básica, a serem contratadas no ACL;
 -	Os valores em MWh foram transformados em MWmédios, notação utilizada no ACL para contratação de energia e, totalizou-se as médias de consumo com perdas das unidades onde chegou-se a um valor de 0,35 MW médios;
 - Com base no histórico de consumo verificado foi realizada a sazonalização do contrato de 0,35 MWmédios visando a melhor distribuição da carga ao longo do ano;
 - Foram considerados padrões mais utilizados pelos agentes de comercialização, como sazonalização de +/-15% e flexibilidade mensal de +/-15% em relação ao montante contratual;
 - Foram utilizadas as tarifas de energia elétrica vigentes na data de 18/01/2021 das distribuidoras locais RGE e COPEL, além das bandeiras tarifárias;
 - Para o mercado livre foram considerados preços de energia elétrica proveniente de fonte incentivada com 50% de desconto na TUSD, verificados no dia 18/01/2021;
 - Como se trata de um consumidor especial é obrigatória a contratação de energia incentivada para migração;
 - Foram considerados preços para um horizonte de 5 anos 2022 a 2026;
 - Como não foram liberados acessos aos contratos de fornecimento de energia considerou-se que a migração de todas as unidades ocorrerá em 01/01/2022;
 - Todos as tarifas e preços na mesma base de janeiro de 2021;
 - Foram considerados os impostos como PIS, COFINS e ICMS, dado que se trata de instituição de ensino e o ICMS é custo, logo foi considerado no estudo.
Reforçando que a sazonalização deve ser realizada anualmente de forma antecipada, normalmente entre os meses de outubro e novembro do ano anterior ao início do período de fornecimento e, com isso, é possível solicitar propostas aos fornecedores de energia elétrica no ACL para esta referida universidade.  
Os preços de mercado utilizados para energia incentivada 50% TUSD são os valores mostrados na abaixo, relativos a data do dia 18/01/2021 (obtidos sob consulta a empresa do ramo).
                                                             Ano   R$/MWh
                                                             2022  233
                                                             2023  197
                                                             2024  183
                                                             2025  170
                                                             2026  160
~~~

## Evolução do Projeto
~~~
<Relate a evolução do projeto: possíveis problemas enfrentados e possíveis mudanças de trajetória. Relatar o processo para se alcançar os resultados é tão importante quanto os resultados.>
~~~

# Resultados e Discussão
### UC1
~~~
Para esta UC existe a necessidade de ajuste no contrato de demanda para o valor de 220 kW, dado que a mesma vem desempenhando valores bem abaixo de 250 kW, atual contrato. De posse dos valores de tarifa atuais vigentes, assim como os encargos e perdas, abaixo são mostradas as economias previstas para os anos de 2022 até 2026 para esta UC, considerando também as bandeiras tarifárias vigentes.
~~~
https://github.com/juliobento9131/IT304S_Trabalho_Parte_2/issues/1#issue-791443223

### UC2
~~~
Para esta UC existe a necessidade de ajuste no contrato de demanda para o valor de 270 kW, dado que a mesma vem desempenhando valores muito acima de 197 kW, atual contrato. De posse dos valores de tarifa atuais vigentes, assim como os encargos e perdas, abaixo são mostradas as economias previstas para os anos de 2022 até 2026 para esta UC, considerando também as bandeiras tarifárias vigentes.
~~~
https://github.com/juliobento9131/IT304S_Trabalho_Parte_2/issues/2#issue-791459933

### UC3
~~~
Para esta UC existe a necessidade de ajuste no contrato de demanda para o valor de 100 kW, dado que a mesma vem desempenhando valores muito acima de 75 kW, atual contrato. De posse dos valores de tarifa atuais vigentes, assim como os encargos e perdas, abaixo são mostradas as economias previstas para os anos de 2022 até 2026 para esta UC, considerando também as bandeiras tarifárias vigentes.
~~~
https://github.com/juliobento9131/IT304S_Trabalho_Parte_2/issues/3#issue-791460823

### UC4
~~~
Para esta UC existe a necessidade de ajuste no contrato de demanda para o valor de 60 kW, com o intuito de somente adequação do valor do contrato que é 53 kW. De posse dos valores de tarifa atuais vigentes, assim como os encargos e perdas, abaixo são mostradas as economias previstas para os anos de 2022 até 2026 para esta UC, considerando também as bandeiras tarifárias vigentes.
~~~
https://github.com/juliobento9131/IT304S_Trabalho_Parte_2/issues/4#issue-791462083

### UC5
~~~
Para esta UC existe a necessidade de ajuste no contrato de demanda para o valor de 230 kW, com o intuito de somente adequação do valor do contrato que é 227 kW. De posse dos valores de tarifa atuais vigentes, assim como os encargos e perdas, abaixo são mostradas as economias previstas para os anos de 2022 até 2026 para esta UC, considerando também as bandeiras tarifárias vigentes.
~~~


### UC6
~~~
Para esta UC existe a necessidade de ajuste no contrato de demanda para o valor de 230 kW, com o intuito de somente adequação do valor do contrato que é 220 kW. De posse dos valores de tarifa atuais vigentes, assim como os encargos e perdas, abaixo são mostradas as economias previstas para os anos de 2022 até 2026 para esta UC, considerando também as bandeiras tarifárias vigentes.
~~~


### TOTAL
~~~
Ao somar a totalidade das UCs, verifica-se os valores de economias previstas para os anos de 2022 até 2026 para esta universidade, conforme segue.
~~~

~~~
Com isso posto, é possível verificar a viabilidade econômica de migração para todas as UC's, com maior economia no final do ciclo considerando os preços de mercado da Tabela 1.
~~~

# Conclusões
~~~
Após análise individual das 6 UCs, foi possível consolidar a viabilidade econômica da migração para o ACL da UFFS – Universidade Federal da Fronteira Sul. Foram apuradas as diferenças cativo x livre para os anos de 2022 a 2026, considerando a aplicação ou não de bandeiras tarifárias. Foi considerado como investimento o emolumento de adesão à CCEE, R$ 7.000,00 a ser pago uma vez pelo cliente para início na CCEE e também os custos de adequação do SMF – Sistema de Medição para Faturamento das unidades, sendo de R$ 32.000,00 (R$ 8.000,00 por unidade) na RGE e R$ 30.000,00 ($ 15.000,00 por unidade) na COPEL, totalizando um investimento médio total de R$ 69.000,00, a depender das características físicas de cada unidade. Por fim, considerando que este investimento fosse quitado em 2022, ano previsto para migração total da universidade, abaixo é mostrado o payback previsto (em meses) contemplando a aplicação ou não de bandeiras, com base no valor da economia prevista para o mês. 

                                                                   Ano 2022
                                                             Investimento   Payback
                                      Bandeira verde         69000          1,62 meses
                                      Bandeira amarela       69000          1,50 meses
                                      Bandeira vermelha 1    69000          1,30 meses
                                      Bandeira vermelha 2    69000          1,18 meses
                                                             
Com esse estudo em questão, é possível solicitar propostas aos fornecedores de energia elétrica no ACL e, com isso a UFFS – Universidade Federal da Fronteira Sul poderia obter as economias previstas conforme colocado no item 1.1.7 e investir em outras áreas onde for mais necessário na universidade. 
~~~

# Trabalhos Futuros
~~~
Este trabalho pode ser estendido a outras universidades públicas ou não para análise de viabilidade de migração ao ACL.
~~~
