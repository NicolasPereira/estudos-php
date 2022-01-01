<!-- Title -->
<h2 align="center">Arquivo de configuração</h2>

<p align="center">
   Entendendo sobre o arquivo de configuração do PHP
</p>    
 <!-- ABOUT THE TOPIC -->
<hr>

O _php.ini_ é o arquivo resposánvel pelas configurações do PHP em seu ambiente de desenvolvimento local ou até mesmo no ambiente de produção.

Neste arquivo é possível parametrizar diversas opções do PHP. 

Para verificar onde o seu arquivo _php.ini_ se encontra instalado é basta criar um arquivo com o código abaixo.
```php
<?php
phpinfo()
```

A função `phpinfo()` irá retornar uma tela parecida com esta:

<div align="center">
    <img src="/assets/fundamentos/php-ini.png" widht="400px" height="240px">
</div>

Para localizar o seu arquivo de configuração basta visualizar o caminho apresentado no retorno do `phpinfo()` no campo **Loaded Configuration File**, no caso da imagem de exemplo o caminho é `etc/php.ini`!

Agora é só abrir o seu arquivo de configuração no seu editor/IDE para visualizar as configurações.

Vamos alterar algumas configurações importantes para o seu **_Ambiente de Desenvolvimento_**. 

As váriaveis abaixo elas serve para exibir os erros do PHP durante a execução do seu programa, é importante habilitar essas configurações para caso tenha algum erro de sintaxe, estouro de memória, drivers e afins você consiga visualizar mais fácil.

`display_error=On`
`error_landing=E_All`

Agora vamos ativar os registros de log do PHP, dessa forma se ocorrer algum erro podemos recorrer aos logs para obter mais detalhes.

`logs_errors=On`
`erros_logs=/tmp/php_erros.log`

Dessa forma ativamos os logs e definimos qual sera o arquivo de erro e em qual local ele ficara salvo. 

A configuração abaixo deve ser muito bem configurada tanto em ambientes de produção quanto de desenvolvimento, vamos alterar o máximo de mémoria que o PHP vai utilizar do nosso computador.

`memory_limit=256M` este valor é em Megabyte.


Agora vamos configurar o tempo de execução máxima de um script php em segundos. 

`max_execution_time=120`

>As duas configurações acima devem ser bem alinhadas pois se utilizarmos muita memória teremos mais gastos de infraestrutura e se aumentarmos mais o tempo de execução de cada script também teremos um custo alto de infraestrutura.


Durante o desenvolvimento as vezes é necessário trabalhar com upload de arquivos, por este motivo vamos também configurar para o PHP aceitar arquivos.

`file_uploads=On`
`post_max_size=100M` - tamanho máximo do corpo de uma requisição, incluindo multiplos arquivos, valor em Megabyte.
`upload_max_filesize=100M`- tamanho máximo de um arquivo que pode ser enviado em Megabyte.


No PHP utilizamos o conceito de sessões para armazenar algumas informações, verificar se um usuário está logado e afins, por isso no `php.ini` podemos aumentar ou diminuir este parâmetro.

`session.gc_maxlifetime = 14000` - este valor é em segundos.

Como dito anteriormente, o _php.ini_ é o arquivo de configuração do PHP, nele você poderá configurar ainda mais coisas como por exemplo drivers específicos de um Sistema de Gerenciamento de Banco de dados. 

Para saber mais sobre o _php.ini_ acesse a [documentação](https://www.php.net/manual/en/ini.list.php).


<p align="center">Made with 💜</p> 