# Projeto `VIABILIDADE ECONÔMICA DE MIGRAÇÃO PARA O ACL DA UFFS – UNIVERSIDADE FEDERAL DA FRONTEIRA SUL`
# Project `ECONOMIC FEASIBILITY OF MIGRATION FOR ACL UFFS - FEDERAL UNIVERSITY OF FRONTIER SOUTH`

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
R: Para primeiro ano a economia estimada foi de 23 a 29% a depender a bandeira tarifária considerada. Os demais anos analisados estão detalhados no arquivo 
Qual é o preço da energia a partir de quando compensa a migração?
R: O Break Even Point ou preço de empate calculado foi de R$370,74 para a RGE e R$340,49 para a COPEL.
Qual a recomendação para uma contratação? (Características de contrato como volume, flexibilidade, modulação, sazonalização).
R: A recomendação é a contratação de 0,35MW médios na modalidade flex com variação de 15% acima ou abaixo.
~~~

## Objetivos do projeto
~~~
<Como seu projeto propôs abordar o problema apresentado.>
~~~

# Recursos e Métodos

## Bases de Dados
`<Elencar bases de dados utilizadas no projeto preferencialmente no formato da tabela a seguir.>`
Base de Dados | Endereço na Web | Resumo descritivo e uso
----- | ----- | -----
Base 1 | http://base1.org/ | `<Descrição da Base 1 e para que ela foi usada no projeto.>`
Base 2 | http://base2.org/ | `<Descrição da Base 2 e para que ela foi usada no projeto.>`

## Ferramentas

`<Elencar ferramentas utilizadas no projeto preferencialmente no formato da tabela a seguir.>`
Ferramenta | Endereço na Web | Resumo descritivo e uso
----- | ----- | -----
Ferramenta 1 | http://ferramenta1.org/ | `<Descrição da Ferramenta 1 e para que ela foi usada no projeto.>`
Ferramenta 2 | http://ferramenta2.org/ | `<Descrição da Ferramenta 2 e para que ela foi usada no projeto.>`

# Metodologia
~~~
<Abordagem/metodologia adotada, incluindo especificação de quais técnicas foram exploradas, tais como: aprendizagem de máquina, análise de redes, análise estatística, ou integração de uma ou mais técnicas.>
~~~

## Detalhamento do Projeto
~~~
<Apresente aqui detalhes da análise. Nesta seção ou na seção de Resultados podem aparecer destaques de código como indicado a seguir. Note que foi usada uma técnica de highlight de código, que envolve colocar o nome da linguagem na abertura de um trecho com `~~~`, tal como `~~~python`.

Os destaques de código devem ser trechos pequenos de poucas linhas, que estejam diretamente ligados a alguma explicação. Não utilize trechos extensos de código. Se algum código funcionar online (tal como um Jupyter Notebook), aqui pode haver links. No caso do Jupyter, preferencialmente para o Binder abrindo diretamente o notebook em questão.>
~~~

~~~python
df = pd.read_excel("/content/drive/My Drive/Colab Notebooks/dataset.xlsx");
sns.set(color_codes=True);
sns.distplot(df.Hemoglobin);
plt.show();
~~~

## Evolução do Projeto
~~~
<Relate a evolução do projeto: possíveis problemas enfrentados e possíveis mudanças de trajetória. Relatar o processo para se alcançar os resultados é tão importante quanto os resultados.>
~~~

# Resultados e Discussão
~~~
<Apresente os resultados da forma mais rica possível, com gráficos e tabelas. Mesmo que o seu código rode online em um notebook, copie para esta parte a figura estática. A referência a código e links para execução online pode ser feita aqui ou na seção de detalhamento do projeto (o que for mais pertinente).

A discussão dos resultados também pode ser feita aqui na medida em que os resultados são apresentados ou em seção independente. Aspectos importantes a serem discutidos: É possível tirar conclusões dos resultados? Quais? Há indicações de direções para estudo? São necessários trabalhos mais profundos?>
~~~

# Conclusões
~~~
<Apresente aqui as conclusões finais do trabalho e as lições aprendidas.>
~~~

# Trabalhos Futuros
~~~
<Indique trabalhos futuros a partir do ponto alcançado.>
~~~
