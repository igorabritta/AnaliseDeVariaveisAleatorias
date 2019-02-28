# MatlabCourse

A ideia desse repositorio é podermos passar uma primeira tarefa para treinar os novos bolsistas e ao mesmo tempo podermos receber feedback e melhorar do ponto de vista acadêmico.

## Módulo 1 

1. Criar duas variáveis Gaussianas ([Distribuição Gaussiana](https://www.inf.ufsc.br/~andre.zibetti/probabilidade/normal.html)) com médias diferentes e com o mesmo número de eventos.

2. Definir qual será o SINAL(Signal) e qual será o RUÍDO DE FUNDO(Background). 

3. Varrer todo range das duas variáveis e ver a porcentagem de eventos que você erra e acerta para cada limiar verificado 
([Curva ROC](http://crsouza.com/2009/07/13/analise-de-poder-discriminativo-atraves-de-curvas-roc/)).

4. Modificar a média das distribuições e verificar o que ocorre com as porcentagens de acerto de sinal e background. 
Depois, definir a média paras variáveis gaussianas, modificar a variância e ver o que ocorre com as porcentagens 
de acerto de sinal e background.

5. Escolher uma média e uma variância qualquer e definir qual o limiar com melhor eficiência x melhor rejeição de background 
e fazer um plot3d ([plot3](https://www.mathworks.com/help/matlab/ref/plot3.html)), com os eixos plot3(var1,var2,rótulo_melhor_limiar) e plotar junto com  plot3(var1,var2,rótulo_truth)

6. Mostrar o histograma bidimensional (hist3) das variáveis.

Dica: Cada evento de sinal deve ter um rótulo = 1 e cada evento de background deve ter um rótulo = 0 (rótulo_truth). Ao passar o limiar por todo range você verifica quem é maior do que o limiar e quem é menor, e então vê se acertou ou errou o evento olhando seu rótulo.

## Módulo 2

Vamos expandir o raciocínio para 2 dimensões:

1. Criar 2 conjuntos bidimensionais: para sinal e ruído; 
2. Varrer o limiar da seguinte forma:

      2.1. Varrer o limiar bidimensional, que será perpendicular a reta que ligar a média dos dois conjuntos (sinal e ruído);
      
      2.1. Varrer o limiar para cada dimensão;
      
3.  Plotar 3 rocs (com seus respectivos melhores SP): 1 pro limiar bidimensional e 2, uma pro limiar de cada dimensão
4.  Verficar qual das abordagens é a melhor.

## Módulo 3

Criar uma apresentação mostrando os resultados e explicando os códigos.
