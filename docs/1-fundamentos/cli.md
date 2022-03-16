<!-- Title -->
<h2 align="center">Command Line do PHP</h2>

<p align="center">
   Entendendo o Command Line do PHP
</p>    
 <!-- ABOUT THE TOPIC -->
<hr>

O PHP possui uma ferramenta muito interessante que é o *command line*, com essa ferramenta você pode interagir com o PHP através do terminal.! 

Digite no seu terminal: 

```bash
php -v
```

O retorno será algo parecido com 

```bash
PHP 8.0.14 (cli) (built: Dec 17 2021 22:21:16) ( NTS )
Copyright (c) The PHP Group
Zend Engine v4.0.14, Copyright (c) Zend Technologies
with Zend OPcache v8.0.14, Copyright (c), by Zend Technologies
```

Com o comando acima é possível descobrirmos qual a versão do PHP está instalada, no meu caso estou utilizando a versão 8.0.14;.

Outro comando interessante é:

```bash
php -a
```

Este comando abre um terminal interativo onde você pode digitar comandos PHP! 

Tente digitar no terminal o comando abaixo e pressionar enter em seguinte

```php
echo "Olá Mundo";
```

O seu resultado no terminal será algo parecido com isso.

```bash
Interactive shell

php > echo "Olá Mundo";
Olá Mundo
php >
```

Para sair do terminal interativo do PHP basta digitar `quit`! 

Um ponto muito importante, dentro do terminal interativo é necessário respeitar a sintaxe do PHP.

<p align="center">Made with 💜</p> 