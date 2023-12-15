# testando API PDV pelo render 

Você deverá utilizar um testador de rotas utilizando o link: [eight-bit-api.onrender.com](https://eight-bit-api.onrender.com) 

# testando API PDV localmente (na máquina) 

# Instalação do Node.js 

Você deverá ter o motor V8 instalado em sua máquina para rodar a aplicação 

# Windows:

Baixe o instalador: Acesse o site oficial do Node.js (https://nodejs.org) e baixe o instalador do Node.js para Windows.

Execute o instalador: Depois de baixar, execute o arquivo do instalador e siga as instruções na tela.

Conclua a instalação: Depois de seguir os passos, o Node.js e o npm (gerenciador de pacotes do Node) devem estar instalados no seu sistema.

# macOS:

Usando o instalador do site oficial: Baixe o instalador do Node.js para macOS no site oficial (https://nodejs.org).

Execute o pacote: Abra o arquivo .pkg baixado e siga as instruções na tela para instalar o Node.js.

Verifique a instalação: Abra o Terminal e digite node -v e npm -v para verificar se o Node.js e o npm foram instalados corretamente.

# Linux:
Usando o gerenciador de pacotes:
Utilizando o terminal:

Para distribuições baseadas em Debian/Ubuntu:

```
sudo apt-get update
sudo apt-get install nodejs
sudo apt-get install npm
Para distribuições baseadas em Red Hat/Fedora:
```

```
sudo dnf install nodejs
sudo dnf install npm
``` 
# Instalação do PostgreSQL 

Você deverá ter o postgreSQL instalado em sua máquina para testar a aplicação localmente 

# Windows:
Baixe o instalador: Acesse o site oficial do PostgreSQL (https://www.postgresql.org/download/windows/) e baixe o instalador para Windows.

Execute o instalador: Após o download, execute o arquivo do instalador. Durante a instalação, você poderá configurar senhas para o usuário administrativo (postgres).

Selecione componentes: Durante a instalação, você pode selecionar os componentes que deseja instalar, como o PostgreSQL Server e o pgAdmin (interface gráfica para gerenciamento).

Conclua a instalação: Siga as instruções na tela para concluir a instalação.

# macOS:
Baixe o instalador: Acesse o site oficial do PostgreSQL (https://www.postgresql.org/download/macosx/) e baixe o instalador para macOS.

Execute o instalador: Após o download, abra o arquivo do instalador e siga as instruções na tela para instalar o PostgreSQL.

Conclua a instalação: O instalador vai guiá-lo pelo processo de instalação, onde você pode configurar a senha do usuário administrativo e outros parâmetros.

# Linux:
Usando o gerenciador de pacotes: Dependendo da distribuição, você pode instalar o PostgreSQL usando o gerenciador de pacotes. Por exemplo:

Para distribuições baseadas em Debian/Ubuntu:

``` 
Copy code
sudo apt-get update
sudo apt-get install postgresql postgresql-contrib
``` 

Para distribuições baseadas em Red Hat/Fedora:

``` 
sudo dnf install postgresql-server
``` 

Configuração inicial: Após a instalação, você pode precisar iniciar o serviço do PostgreSQL e configurá-lo usando comandos como sudo systemctl start postgresql e sudo systemctl enable postgresql.

# Criação de credenciais env 

Você deverá criar na raiz do projeto um arquivo chamado ".env" e seguir o exemplo do arquivo .env.example 

Algumas rotas utilizam credenciais específicas para hospedagem de imagens na nuvem e envio de e-mails automáticos através de servidores SMTP, ou seja, para utiliza-las você deverá solicitar as credenciais em anjosdelacerda@gmail.com ou https://www.linkedin.com/in/lacerda-fernando/

Caso não queria testar essas rotas em específico, a falta dessas credenciais apenas te impedirá de criar produtos hospedando imagens (o campo não é obrigatório) e os e-mails de confirmação de pedidos não será enviado.

# Testando as rotas

Para testar as rotas basta que você importe o arquivo 'Insomnia_2023-12-02.json' que esta na raiz deste repositório dentro do seu testado de rotas (insomnia, postman). As rotas já estão separadas por classes.

Recomendamos que primeiramente se crie um usuário em 'USER' e depois faça um login, pois assim as credenciais para rotas protegidas serão liberadas, as rotas já estão configuradas para receberem o token da rota de login.

