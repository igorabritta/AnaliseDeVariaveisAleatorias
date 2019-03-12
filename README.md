# Curso para iniciar o uso de Matlab para análise de variáveis aleatórias

A ideia desse repositorio é podermos passar uma primeira tarefa para treinar os novos bolsistas e ao mesmo tempo podermos receber feedback e melhorar do ponto de vista acadêmico.

## Módulo 1 

1. Criar duas variáveis [Gaussianas](https://www.inf.ufsc.br/~andre.zibetti/probabilidade/normal.html), f(x) e g(x) com [médias](http://www.est.ufmg.br/~marcosop/est031/aulas/Capitulo_4_1.pdf) diferentes e com o mesmo número de eventos. 

2. Definir qual será o Sinal (*Signal*) e qual será o Ruído de Fundo(*Background*).

3. Varrer todo *range* das duas variáveis e ver a porcentagem de eventos que você erra e acerta para cada limiar verificado 
([Curva ROC](http://crsouza.com/2009/07/13/analise-de-poder-discriminativo-atraves-de-curvas-roc/)).

4. Modificar média, [variância](http://www.est.ufmg.br/~marcosop/est031/aulas/Capitulo_4_1.pdf) e número de eventos das distribuições e verificar o que ocorre com as porcentagens de acerto de *signal* e *background*. Criar uma curva ROC e avaliar o efeito dessas variações.

5. Escolher uma média e uma variância qualquer e definir qual o limiar com melhor eficiência de sinal x melhor rejeição de *background* através do [critério SP](https://drive.google.com/file/d/1VifytdIoQkYvuBUzW5Ybgk0QH36XDAP3/view (Página 98)) (Página 98).

6. Exibir o histograma das variáveis geradas juntamente com o limiar escolhido.

7. Criar um plot3(x,y,z) onde x e y correspondem a variação da média em determinado intervalo([-m,m]) com passo arbitrário p e z corresponde ao melhor SP. 

8. Repita o item anterior agora utilizando a variância(atentar para o intervalo de variação).

9. Com a média e a variância utilizada no item 5, executar o algoritmo *n* vezes e gerar uma distribuição com o melhor limiar de cada iteração. Variar o número de eventos de cada conjunto de dados e avaliar o impacto desta alteração.

##### Dica: Cada evento de *signal* deve ter um rótulo = 1 e cada evento de *background* deve ter um rótulo = 0 (rótulo_truth). Ao passar o limiar por todo range você verifica quem é maior do que o limiar e quem é menor, e então vê se acertou ou errou o evento olhando seu rótulo.

## Módulo 2

Vamos expandir o raciocínio para 2 dimensões:

1. Criar 2 conjuntos bidimensionais gaussianos: para sinal f(x,y) e ruído g(x,y);

2. Varrer o limiar da seguinte forma:
   - Varrer o limiar para cada dimensão;  
   - Varrer o limiar bidimensional, que será perpendicular a uma reta suporte que liga a média dos dois conjuntos (sinal e ruído);
   - Repetir o item anterior *n* vezes porém estimando as médias dos conjuntos de dados utilizados na construção da reta suporte. Após isso avaliar a dispersão do melhor SP em relação ao SP calculado com a média verdadeira. Analisar o impacto do número eventos.
   
3. Escolher média e variância fixa e exibir o histograma bidimensional das variáveis geradas juntamente com o limiar escolhido.

4. Criar um plot3(x,y,z) onde x e y correspondem a variação da média em determinado intervalo([-m,m]) com passo arbitrário p e z corresponde ao melhor SP. 

5. Repita o item anterior agora utilizando a variância(atentar para o intervalo de variação).

6. Plotar 3 rocs (com seus respectivos melhores SP): 1 pro limiar bidimensional e 2, uma pro limiar de cada dimensão;

7. Verificar qual das abordagens é a melhor.

## Módulo 3

Agora para ter uma experiência uma pouco mais palpável do que podem ser variáveis e o porque indentificar com mais eficiência e menor falso alarme é uma tarefa importante vamos usar o [Iris DataSet](https://archive.ics.uci.edu/ml/datasets/iris).

1. Repetir o módulo 1 usando a variável 'Sepal Length', sendo a classe 'Iris Setosa' e 'Iris Versicoulour' como f(x) e g(x), respectivamente.

2. Repetir o módulo 2 usando as variáveis 'Sepal Length' e Sepal width' como Primeira e Segunda dimensão, respectivamente, e as as mesmas classes do exércio 1.

3. Executar esses exercícios mudando as outras variáveis e/ou as classes com o intuito de familiarizar-se com diferentes cenários.

4. O que fazer para separar mais de 2 classes? Respodam sem implementar, somente com ideias do que poderia ser feito para resolver esse tipo de situação.

## Módulo 4

Criar uma apresentação com:

0 - Sumário


1 - Introdução


2 - Desenvolvimento


3 - Resultados


4 - Conclusão

##### Dica: A apresentação deve conter o número dos slides e as figuras devem conter legenda e identificação dos eixos.


# Tópicos correlatos que podem ser úteis

1. [Correlação de Pearson](https://www.inf.ufsc.br/~vera.carmo/Correlacao/Correlacao_Pearson_Spearman_Kendall.pdf)

2. [Covariância](http://www.portalaction.com.br/probabilidades/42-covariancia-e-coeficiente-de-correlacao)

3. [GitHub Tutorial](https://guides.github.com/activities/hello-world/)

4. [Git Tutorial](https://guides.github.com/introduction/git-handbook/)

5. [Sintaxe básica para escrever o ReadMe](https://help.github.com/en/articles/basic-writing-and-formatting-syntax)

6. [Matlab Tutorial](https://web.eecs.umich.edu/~aey/eecs451/matlab.pdf)

7. [Matlab Machine Learning Project using Iris Dataset](https://github.com/akulagrawal/ML-with-Matlab)

# Open Data sets

Site com inúmeros banco de bados abertos e muito utilizados pela comunidade acadêmica:
https://archive.ics.uci.edu/ml/datasets.html

[Iris DataSet](https://archive.ics.uci.edu/ml/datasets/iris): Este é talvez o banco de dados mais conhecido encontrado na literatura sobre reconhecimento de padrões. O conjunto de dados contém 3 classes de 50 instâncias cada, onde cada classe se refere a um tipo de planta da íris. Uma classe é linearmente separável das outras duas; já as outras duas não são linearmente separáveis uma da outra.
