## Requisitos

Os requisitos são um navegador, preferencialmente o Google, o Visual Studio Code, dentro do Visual Studio Code a extensão Python, pelo terminal a criação da pasta "venv" e a instalação e execução do Flask, para poder acessar o website pelo navegador.

### Visual Studio Code

É possível instalar o Visual Studio Code pelo website, pesquisando em um navegador ou diretamente [aqui](https://code.visualstudio.com/download).

### Extensão Python

Dentro do Visual Studio Code, deve-se, dentro da aba de extensões, pesquisar "Python" e instalar a primeira extensão a fizer sua aparição.

### MySQL Workbench

Baixe o MySQL Workbench por [aqui](https://dev.mysql.com/downloads/installer/), aguarde o término do download e clique para instalar, aceite a intalação de todas as extensões e termine a instalação. Dentro do MySQL abra o serviço "localhost", coloque a senha ***fatec*** e o usuário ***root***

Dentro do serviço cole execute com o "raio" na parte superior o seguinte comando:

```
create database contatos;
use contatos;
create table contatos(
    email varchar(60),
    assunto varchar(60),
    descricao varchar(255)
);
```

### venv

A pasta venv deve ser criada toda vez na qual esses arquivos foram descarregados em um aparelho computador diferente. Com a extensão Python instalada, abrir o terminal do Visual Studio Code, colocar os seguintes comandos:

```
apt get update
py -m venv venv
```
Agora deve-se entrar no terminal "PowerShell" do Windows como **administrador** e digitar o seguinte comando:

```
Set-ExecutionPolicy -ExecutionPolicy AllSigned
```

Logo em seguida ele irá questionar se desejas mesmo executar o comando, deve-se enviar a letra **A** para **confirmar todos**.

Deve-se entrar agora na pasta venv, digitando o seguinte comando no terminal do Visual Studio Code, que anteriormente foi aberto:

```
.\venv\Scripts\activate
```

### Requerimentos

Ainda no terminal, para instalar os requerimentos para visualizar o website, enviar o seguinte comando:

```
pip install -r requirements.txt

Para visualizar o website deve-se executar o Flask, seguindo o comando abaixo:

```
Flask run
```

Agora, aparecerá um link em formato de protocolo IP, onde, segurando o botão **Control**, deve-se clicar com o botão esquerdo do mouse.
Para navegar pelas abas do website pode-se clicar nos links em formato de nome no canto superior direito da tela.
