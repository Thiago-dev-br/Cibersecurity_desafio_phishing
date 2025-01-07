# Cibersecurity_desafio_phishing
Metodo de clone do site para captura de login e senha

Todo o projeto foi realizado utilizando o kali Linux, sendo necessário a virtulização da ISO.

#Virtulização:

1º Passo – Realizar o download do Oracle Virtualbox 4.0.2 para Microsoft Windows

https://www.oracle.com/br/virtualization/technologies/vm/downloads/virtualbox-downloads.html

![image](https://github.com/user-attachments/assets/26ce003b-9776-4da1-be11-338ac14b4126)

Na imagem, mostra o binário do Oracle Virtualbox 4.0.2 para Microsoft Windows e o arquivo de Extension Pack também. Faça o download dos dois arquivos, pois extension pack iremos tratar em outro artigo a sua utilização.

Após o download, se executar um duplo clique sobre o arquivo Virtualbox-4.0.2-69518-Win.exe, caso pegue uma versão atualizada no site, o nome será outro.

2º Passo – Iniciando a instalação do Oracle Virtualbox 4.0.2 para Microsoft Windows
Iniciando a instalação do Oracle Virtualbox 4.0.2 para Microsoft Windows

![image](https://github.com/user-attachments/assets/5b567561-699b-4eb6-ae82-a431bfee8b42)

Esta é a tela inicial de setup do Instalador do Oracle Virtualbox, basta clicar em NEXT.

3º Passo – Selecionar as características de instalação
Selecionar as características de instalação

![image](https://github.com/user-attachments/assets/36f0240d-8db3-4036-83ce-a3d8bf0ddf69)

Nessa tela, iremos selecionar os componentes de instalação do Virtualbox, verifique se todos estão selecionados.

Os componentes que serão instalados são para as principais funcionalidades do Virtualbox, tais como:

#Virtualbox USB Support

Permite o compartilhamento das portas USB da sua máquina com as máquinas virtuais.

#Virtualbox Network

Permite a realização de Bridge em sua placa de rede, para posteriormente colocar as máquinas virtuais dentro da sua rede local ou corporativa.

#Virtualbox Python Support

São as bibliotecas escritas em Python para os recursos do VirtualBox. Após verificar que estão todas selecionadas, clique em NEXT.

Observação
Nessa tela também é possível realizar a alteração do caminho que será instalado o virtualbox, caso queira colocar o virtualbox em uma pasta exclusiva ou até mesmo em outra unidade lógica da sua máquina, clique no botão BROWSE para alterar o caminho de instalação.

4º Passo – Criação dos Atalhos no sistema operacional

![image](https://github.com/user-attachments/assets/27f0d8c5-1f55-4504-acd5-d7a2afaab3bf)

Criação dos Atalhos no sistema operacional

Nesta tela, existem dois check-box apenas para você especificar se quer ou não criar um atalho para o aplicativo Oracle Virtualbox no seu desktop e quick launch.

Para prosseguir, clique em NEXT.

5º Passo – Tela de aviso de interrupção temporária da sua placa de rede

![image](https://github.com/user-attachments/assets/9727e9f9-88f2-4a78-b7c2-b13ac034fee4)

Tela de aviso de interrupção temporária da sua placa de rede

Neste passo da instalação, a tela acima apenas menciona que irá interromper por alguns instantes a sua placa de rede, justamente para a criação das bridges sobre a sua placa de rede. Lembra no passo 3 que selecionamos as opções do Oracle Virtualbox Network, então, ele está trabalhando neste momento, e posteriormente você irá verificar as configurações de rede.

Para detalhar mais um pouco, as BRIDGES são uma forma de emular uma outra interface de rede sem a necessidade de uma placa de rede física adicional, ou seja, posteriormente, você poderá ter dois ou mais IPs sobre uma única placa de rede física.

Para saber mais detalhes sobre Network Bridge, consulte este site: Kioskea.net Após matar a curiosidade sobre Network bridge, clique em NEXT.

6º Passo – Prosseguir a instalação

![image](https://github.com/user-attachments/assets/53333805-0250-49a4-9645-6de68b705e1c)

Prosseguir a instalação

Agora, o virtualbox irá apenas mencionar para prosseguir a instalação, clique em INSTALL.

7º Passo – Andamento da instalação

![image](https://github.com/user-attachments/assets/06ab6dd4-53ce-45ea-9978-29472f184b05)

Andamento da instalação

Essa tela pode demorar alguns minutos para realizar a instalação completa do Oracle Virtualbox, portanto, até aparecer a próxima tela que está no próximo passo, vou publicar alguns links interessantes para conhecer um pouco mais sobre o Oracle Virtualbox, segue:

1. Virtualbox – Site oficial 2. Wikipédia do Virtualbox 3. Joel Texeira – Virtualbox – Virtualização eficaz e Open Source 4. Oficina da net – Tutorial sobre Virtualbox 5. Hardware.com.br – Usando o Virtualbox

8º Passo – Finalização da Instalação

![image](https://github.com/user-attachments/assets/ec18c4dc-80df-4b27-b28c-adcc235a9f0a)

Finalização da Instalação

Bom, após algumas leituras dinâmicas sobre os sites acima, chegou o final da instalação do Oracle Virtualbox 4.0.2, e neste momento, já estamos adeptos a utilizar os recursos de virtualização do Oracle virtualbox.

Ao clicar em FINISH, a nossa instalação chega ao final. Sem crise e complicação.

Para quem está utilizando o Microsoft Windows 7, o acesso ao aplicativo será através do caminho abaixo:

INICIAR > TODOS OS PROGRAMAS > Oracle VM Virtualbox > Virtualbox

A tela de apresentação do aplicativo é mostrada abaixo:

![image](https://github.com/user-attachments/assets/5edc72b5-a94a-45e1-ac6d-1e16af79a9bb)

#Download e instalação Kali Linux:

https://www.kali.org/get-kali/#kali-platforms

![image](https://github.com/user-attachments/assets/c465743d-e645-4042-b592-18e31d5bac7f)

Passo a passo da instalação:
Para instalar o Kali Linux usando uma imagem ISO no VirtualBox, siga os passos abaixo:

1° Baixe a imagem ISO de instalação do Kali Linux no site oficial, acessando a seção de download.
Instale o VirtualBox em seu sistema operacional, se ainda não o fez.
2° Abra o VirtualBox e clique em "Novo" para criar uma nova máquina virtual.
3° Escolha um nome, selecione o tipo "Linux" e a versão "Debian 64-bit" para o Kali Linux.
4° Alocando memória (sugere-se pelo menos 2GB).
5° Crie um disco rígido virtual (escolha VDI e faça o tamanho dinâmico ou fixo, com pelo menos 20GB).
6° Selecione a nova máquina virtual criada e clique em "Configurações".
7° Vá até "Armazenamento", clique em "Vazio" sob "Controlador: IDE" e adicione a ISO do Kali Linux.
8° Salve as configurações e inicie a máquina virtual.
9° Siga as instruções na tela para concluir a instalação do Kali Linux.


#Inicialização do projeto no Kali Linux:

![image](https://github.com/user-attachments/assets/9c83bda0-a186-4ae3-977a-69332e8abab6)

A ferramenta utilizada nesse projeto é o Setoolkit, e sendo necessário o seguinte passo caso não tenha no kali:


Abra o terminal e execute o seguinte comando e precione enter:   sudo apt update
  
![image](https://github.com/user-attachments/assets/a5b780f2-e89f-46d6-ac68-8bfd07d12631)

Será realizado o update no kali:

![image](https://github.com/user-attachments/assets/23afbe0c-44ef-45ba-878e-090501694374)

Após finalizar o update, executar o comando a seguir e precione enter:   sudo apt install set

![image](https://github.com/user-attachments/assets/31809268-244f-4c64-8d62-7e0fcfb482c4)

#Executando o SETOOLKIT

Inicialize o SETOOLKIT com o comando e precione enter: sudo setoolkit 

![image](https://github.com/user-attachments/assets/f706cdb0-10dc-47d2-aab3-f3869b8d99f0)

Digite a opção 1 (Social-Engineering Attacks)

![image](https://github.com/user-attachments/assets/34287a4a-3d2d-4ec1-8851-0d30c2ccd53c)

Digite a opção 2 (WebSite Attack Vectors)

![image](https://github.com/user-attachments/assets/95d84b81-ce4d-49ff-a21c-70783e724943)

Digite a opção 3 (credential attack method)

![image](https://github.com/user-attachments/assets/1731d7ee-270c-4aa2-b73c-76a80cf7ade3)

Digite a opçãoo 2 (Site cloner)

![image](https://github.com/user-attachments/assets/380c12b3-98bc-4485-b11d-5fc2b84b4974)

O Ip definido é da sua maquina virtual e será o seu servidor para coletar os dados: (192.168.1.230), clique em enter para continuar
Insira o site que deseja clonar (utilizar obrigatoriamente http://)

![image](https://github.com/user-attachments/assets/78387eb5-f62b-45e8-a13c-b296914a2d4b)


Após a clonagem o site, abrir o navegador e inserir o IP do seu servidor (192.168.1.230)

![image](https://github.com/user-attachments/assets/fc6eadb4-59bd-4b0f-bf97-9b3c57a386ea)

O site utilizado, foi da plataforma Alura: http://www.alura.com.br/loginForm

![image](https://github.com/user-attachments/assets/9535d0af-9e78-4745-86cc-1d270cec6de1)

Após inserir as informações de login e senha, será feito a coleta das informações e o site oficial irá abrir

![image](https://github.com/user-attachments/assets/1c4a968d-8ceb-41e6-9a02-f129529cb4c5)






