<!-- Title -->
<h2 align="center">Comandos de Saida (Output)</h2>

<p align="center">
   Vamos aprender comandos de saída do PHP, para imprimir informações na tela
</p>    
 <!-- ABOUT THE TOPIC -->
<hr>

Durante o seu dia a dia será necessário imprimir as informações manipuladas para o usuário, em exemplos anteriores neste tutorial utilizamos o `echo` mas existem algumas outras formas.

>Ponto de atenção: No momento não se preocupe entender sobre variáveis, o que o código está fazendo mas sim entender sobre a diferença de cada tipo de output! 
>
>Em breve iremos entender o que é uma variável e cada trecho de código apresentado aqui. 
>
O `echo` é um comando que você pode imprimir uma ou mais váriaveis, no código é um exemplo:

```php
<?php
$mundo = "mundo";
echo 'Olá'.PHP_EOL.$mundo;
```

O retorno seria algo como: 
```bash
Olá
mundo
```

O `PHP_EOL` significa `PHP END OF LINE` e sua função é realizar a quebra de linha.

O comando `print`, também pode ser utilizado para imprimir informações do tipo `string`;


```php
<?php
print "Olá Mundo";
```

O `var_dump` é uma função que vai te ajudar muito para debugar variáveis, com o `var_dump` é possível ter informações detalhadas da váriavel passada como parâmetro.

```php
<?php
$nomes = ['Nicolas', 'Arthur', 'Daniel', 'Marcel'];
var_dump($nomes);
```

O resultado será:

```bash
array(4) {
    [0]=> string(7) "Nicolas"
    [1]=> string(6) "Arthur"
    [2]=> string(6) "Daniel"
    [3]=> string(6) "Marcel"
}
```

Por fim, temos o `print_r`, essa função imprime o conteúdo de forma detalhada da mesma forma que o `var_dump` porém o seu diferencial é que exibe o conteúdo de forma alinhada e ocultando os tipos de dados

```php
<?php
$nomes = ['Nicolas', 'Arthur', 'Daniel', 'Marcel'];
print_r($nomes);
```

o resultado será:

```bash
Array (
    [0] =>  Nicolas
    [1] =>  Arthur
    [2] => Daniel
    [3] => Marcel
)
```

<p align="center">Made with 💜</p> 