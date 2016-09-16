# Week 0 - Resumo em Português

## ASCII

Quando aprendemos notação binária, vimos como representar uma gama inteira de números utilizando apenas os caracteres 0 e 1. Agora vamos usar notação binária para representar TEXTO, LETRAS, etc. Mas por que faríamos isto? Bom, um computador, no fim das contas, entende apenas 0's e 1's, uma vez que estes podem ser representados facilmente por utensílios eletromagnéticos.  

Imagine, por exemplo, que a memória de seu computador é uma mesa gigante com várias lâmpadas, onde cada lâmpada desligada representa um 0, e cada lâmpada ligada representa um 1. É mais ou menos assim. Na vida real, computadores utilizam capacitores que, em uma baixa carga de energia, representam um 0, e em alta carga de energia, representam um 1.  

De qualquer forma, precisamos de uma notação que entregue nossas informações (texto, letras, etc) de uma forma que seja entendida pelo hardware.  

Nós temos, em nosso alfabeto, cerca de 25 letras. Cada uma destas letras é representada por um número. Bom, isto parece o bastante para nós. Mas neste sistema, não podemos diferenciar letras minúsculas de maiúsculas. Isso sem contar acentos, pontos, exclamação, etc. No fim das contas, precisamos de toda uma representação em notação binária que informe ao computador que temos um "!", ou um espaço, ou mesmo um "&".  

### American National Standards Institute  

Voltando ao ano de 1960, isto era realmente um problema. Empresas diferentes de tecnologia estavam usando diferentes "tabelas de caracteres" para representar estas coisas dentro do seu hardware. Isto dificultava muito a comunicação entre estas máquinas.  

O American National Standards Institute (ANSI) formou um comitê para desenvolver uma tabela padrão. E em 1963, o American Standard Code for Information Interchange (ASCII) foi criado.  

O padrão ASCII foi desenhado como um encoding de 7 bits, o que significa que cada caractere da tabela é um conjunto de 7 números em notação binária. Esta tabela pode, enfim, armazenar 128 caracteres em formato 7 bits encoding.  

Considerando que usam-se 95 para representar letras maísculas, minúsculas, pontuação e espaço, o que se faz com os 33 caracteres que sobram?

Nesta época já se encadeava um crescimento de máquinas de tele-comunicação, e estas máquinas precisavam de caracteres especiais nestes serviços, como por exemplo, de pular uma linha, ou de recuar um parágrafo, ou mesmo a famosa tecla "backspace" para voltar um caractere. Estes caracteres são chamados de caracteres de controle, e eles constituem o resto do ASCII.