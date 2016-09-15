# Week 0 - Resumo em Português

## Binários

Na escola você aprendeu a escrever números. A princípio te ensinaram este conjunto de números:  

```
0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9
```

E, com este conjunto de números você aprendeu a criar combinações entre eles para representar números maiores do que 9.  

```
52 | 437
```

Esta maneira de escrita de números possui um nome: notação decimal. "Decimal" provém do latim "decem", que significa 10. O 10 é um número bastante especial na notação decimal. Vamos analisar o número 437 escrito em notação decimal:  

Nós podemos quebrar este número da seguinte maneira:  

```
400 + 30 + 7
```

E esmiuçá-lo mais ainda com expressões:  

```
(4x100) + (3x10) + (7x1)
```

Acompanhando isso, podemos perceber várias potências de 10 neste padrão:  

```
(4x10^2) + (3x10^1) + (7x10^0)
```

Porém, a notação decimal NÃO é a única maneira de representar números.  

```
__0__ | __1__ | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9
```

Apenas utilizando os números destacados, nós possuímos uma outra forma de representação: a notação binária. Agora que temos 0 e 1 em nosso conjunto, 2 será nosso número especial. "Binário" vem de "bi" que significa 2. Agora em vez de termos casas decimais com seus lugares para 1, 2, 3, 4, etc, nós temos casas com potências de 2.

```
128 | 64 | 32 | 16 | 8 | 4 | 2 | 1
```

Assim, podemos dizer que 10, interpretado em notação binária, seria na verdade 2. Para representarmos o número 4, por exemplo, escreveríamos 100.  

Para praticar melhor, vamos fazer a leitura de um número grande em notação binária e traduzí-lo para notação decimal:  

```
101110011
```

Para facilitar, vamos representar as potências em suas devidas casas de nosso número:  

```
|  1  |  0  |  1  |  1  |  1  |  0  |  0  |  1  |  1  |
| 2^8 | 2^7 | 2^6 | 2^5 | 2^4 | 2^3 | 2^2 | 2^1 | 2^0 |
```

Se resolvermos a matemática, teríamos os lugares de nossas "casas binárias":  

```
|  1  |  0  |  1  |  1  |  1  |  0  |  0  |  1  |  1  |
| 256 | 128 | 64  | 32  | 16  |  8  |  4  |  2  |  1  |
```

Agora, finalmente, se multiplicarmos tudo junto, teríamos a seguinte representação:  

```
(1x256) + (1x64) + (1x32) + (1x16) + (1x2) + (1x1)
```

Nosso grande número, representado em notação decimal, seria: *371*.  

Agora, faremos algo grandioso. Transformaremos um número em notação decimal para notação binária, algo muito malandrinho, visto que partimos de um número baseado em potências de 10 para um número baseado em potências de 2.  

Aqui temos o número 237 em notação decimal:

```
2 3 7
```

Para dar início à minha tradução, eu procuro a *maior* potência de 2 que seja *menor* que o próprio número. Neste caso, *128*. Assinemos a casa representante com um número 1.  

```
|  0  |  1  |  0  |  0  |  0  |  0  |  0  |  0  |  0  |
| 256 | 128 | 64  | 32  | 16  |  8  |  4  |  2  |  1  |
```

Agora subtraímos *237*, nosso número, ao que acabamos de assinalar, que é *128*. Temos restantes *109*. Então repetimos o processo e assinalamos a próxima *maior* potência de 2 que é *menor* que *109*:  

```
|  0  |  1  |  1  |  0  |  0  |  0  |  0  |  0  |  0  |
| 256 | 128 | 64  | 32  | 16  |  8  |  4  |  2  |  1  |
```

Subtraímos *109* com *64* e temos ainda *45*. Novamente, a *maior* potência de 2 que é *menor* do que *45* é *32*:  

```
|  0  |  1  |  1  |  1  |  0  |  0  |  0  |  0  |  0  |
| 256 | 128 | 64  | 32  | 16  |  8  |  4  |  2  |  1  |
```

Subtraímos nosso *45* por *32* e restam agora apenas *13*. Temos que *8* é nossa potência da vez:  

```
|  0  |  1  |  1  |  1  |  0  |  1  |  0  |  0  |  0  |
| 256 | 128 | 64  | 32  | 16  |  8  |  4  |  2  |  1  |
```

Subtraímos de novo. *13* - *8* é *5*. A casa da vez vira o a potência *4*:  

```
|  0  |  1  |  1  |  1  |  0  |  1  |  1  |  0  |  0  |
| 256 | 128 | 64  | 32  | 16  |  8  |  4  |  2  |  1  |
```

Agora só nos resta o número *1*. Assinalemo-no:  

```
|  0  |  1  |  1  |  1  |  0  |  1  |  1  |  0  |  1  |
| 256 | 128 | 64  | 32  | 16  |  8  |  4  |  2  |  1  |
```

Eis nosso número 237 traduzido para notação binária: *011101101*.  

O que você provavelmente não imagina é que todas as operações de multiplicação, adição, divisão e subtração podem ser também feitas entre números binários. Vejamos um exemplo:  

```
  1101101
+ 1010110
```

Da mesma maneira como fazemos numa operação entre decimais, fazemos entre números binários. A única diferença é que carregamos um *1* quando a operação *dentro da casa ultrapassa o número um*.  