# _CLI_ powers

Uma das primeiras formas de se comunicar com computadores foi através de texto.
Estes primeiros terminais eram conectados a impressoras de telégrafo ([teletipos](https://pt.wikipedia.org/wiki/Teletipo)) que imprimiam em papel o que lhes era pedido.
Até hoje pode-se encontrar resquício disso, o termo _tty_ é uma abreviação para teletipo (_teletype_ em inglês) que também é um nome para terminal.

Mais tarde, monitores com a tecnologia de [tubos de raios catódicos (CRT)](https://pt.wikipedia.org/wiki/Tubo_de_raios_cat%C3%B3dicos) foram conectados a computadores.
A transição foi simplesmente trocar o papel pela tela. Ao invés de imprimir em tinta, imprimia-se no monitor.
As vantagens mais óbvias estavam na economia de papel e velocidade em que a informação era impressa na tela.

Como a programação consiste em escrever textos para serem interpretados por computadores,
essa interface de comandos, há tanto tempo criada, ainda se mostra bastante prática.

## Shell

A camada responsável por interpretar os comandos do usuário para a máquina é chamada de _shell_.

## `bash`

A linguagem de comandos `bash` (que é escrita em _C_) está presente na maioria dos sistemas operacionais descendentes ou inspirados no _Unix_.
O _macOS X_ e diversas distribuições _Linux_ são exemplos desses sistemas.

[Mais...](shell/bash.md)

## Comandos

## `ls`

O comando `ls` lista o conteúdo do diretório.
Se você acabou de abrir o seu emulador de terminal, provavelmente o que lhe será apresentado como reposta é o conteúdo de seu diretório _home_.

![ls no diretório home](media/ls.gif)

Este diretório que é seu "lar" (_home_) é representado também como til (`~`).
O motivo para isto é histórico, os teclados dos anos 70 (ADM-3A) para se digitar o til utilizava-se a tecla _home_.

[Mais...](file-system/ls.md)

## Parâmetros

Ou também chamados de argumentos, são valores informados à direita de algum comando.
estes parâmetros são repassados para o comando que tem então seu comportamento alterado.

O uso de parâmetros é bastante intuitivo,
cada palavra ou número separada por um ou mais espaços em branco (` `) será considerada um parâmetro diferente.

Existem outros caracteres que tem uma importância especial para o `bash`, que vai além do seu significado literal.
Portanto são tratados de uma forma diferenciada e não são repassados como parâmetros.
Para ver a lista completa destes caracteres, veja a sessão de [caracteres especiais para o bash](shell/bash.md#caracteres-especiais).

Nos casos onde algum destes caracteres deveria fazer parte do parâmetro que você quer passar, a solução é simples:
basta colocar o parâmetro todo entre aspas simples (`'`), exemplo:
```bash
echo 'Olá mundo!'
```

Outra forma de fazer o mesmo é utilizando a barra invertida (`\`) antes do caractere que deveria ser ignorado por esse tratamento especial do `bash` e só repassada adiante.
Exemplo:
```bash
echo Olá\ mundo\!
```

Neste exemplo, o espaço logo após a palavra `Olá` está sendo ignorado pelo interpretador `bash` e simplesmente entendido como parte do parâmetro, da mesma forma que o ponto de exclamação.
Por causa deste comportamento, a barra invertida também é chamada de caractere de escape.

[Mais...](shell/bash.md)

## `cd`

- `cd /`

- `cd`

- `cd -`

## `pwd`

## _Autocomplete_

## `file`

## `locate`

- `updatedb`

## `mv`

## `cp`

## `rm`

## `mkdir`

## `rmdir`

## `touch`

- atualiza a data de edição de um arquivo

- caso não exista o arquivo requisitado, cria o arquivo vazio

## `history`

## Control C

## `whatis`, `man`

## Flags

## status retorno comandos
