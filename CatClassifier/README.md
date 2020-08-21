O que nosso modelo fez? De fato, o vetor de entrada x é substituído primeiro ￼e, em seguida, z é substituído na função sigmóide, para que o valor de entrada possa ser convertido em uma probabilidade p.Se p for maior que 0,5, podemos julgar que a imagem é um gato, caso contrário, não é um gato.

Portanto, os parâmetros w e b são muito importantes e determinam o desempenho do nosso modelo!

Como determinar os parâmetros w e b, usando rede neural!

Como a rede neural determina os parâmetros w e b? Através da comunicação para a frente e para trás!

A propagação direta é a primeira a passar pelo processo discutido acima, do vetor de entrada à probabilidade. Em seguida, introduzimos o conceito de uma função de custo ( denotado aqui por L ) . A função de custo é uma função que calcula o "gap" entre o valor previsto e o valor verdadeiro. Por derivating esta função de custo, obtemos dw e db (derivados por w e b, respectivamente) )

A propagação de retorno é a chave para determinar os parâmetros w e b! Como atingir o objetivo de otimização de parâmetros, diferenciando a função de custo? Esse processo é chamado descida de gradiente , especificamente, se você deseja ajustar os parâmetros w, então w da derivada L, para fornecer DW, então use ￼para substituir o original na realização com a otimização dos parâmetros. Aqui ￼está nossa própria definição de taxa de aprendizado (learning_rate) , quanto maior o valor, mais rápido o ajuste w, como escolher a taxa de aprendizado apropriada para este artigo não ser discutido.

Em outras palavras, o processo de ajuste de parâmetros é chamado propagação reversa, e o método de ajuste de parâmetros é chamado descida de gradiente.