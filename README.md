# Desafio-Phishing
Este desafio faz parte do Bootcamp Santander/Dio.me


# Phishing para captura de senhas do Facebook – Santander/DIO.me

### Sistema Operacional e Ferramentas:
- Kali Linux
- Setoolkit
### Configurando o Phishing no Kali Linux
#### Acesse seu kali Linux, após logar no sistema acesse o terminal clicando na tela preta (apontado pela seta vermelha)
![image](https://github.com/user-attachments/assets/c960d1c2-1593-4512-b35d-83d33b1652fe)

ou usando as teclas de atalho ctrl + alt + t

#### Agora vamos elevar os privilégios:
- Acesso root: ``` sudo su ```
 
entre com a senha do root

![image](https://github.com/user-attachments/assets/8a27ea9b-3985-4bd4-9508-ecbe7caee6af)

- Iniciando o setoolkit: ``` setoolkit ```

Basta digitar o nome da ferramenta: setoolkit

![image](https://github.com/user-attachments/assets/2c1ab697-ee40-4977-bf95-b6efadf20b1e)
 
Logo após, aparecerá essa imagem, que muda toda vez que acessamos a ferramenta:

![image](https://github.com/user-attachments/assets/d748267a-bb3e-495c-9c27-33844503db13)

 
Em seguida, aparecerá um menu para selecionarmos qual opção queremos, de 1 a 6, caso queira sair da ferramenta, usar o 99.

![image](https://github.com/user-attachments/assets/2ae05597-92bc-47c3-8325-9bcf8bcd4ec7)

 
- Tipo de ataque: vamos escolher a opção 1) ``` Social-Engineering Attacks ``` e teclar enter.

![image](https://github.com/user-attachments/assets/7e1b91af-e31a-484a-acf2-1ed3cb6b5a6e)

 
Na próxima tela aparecerá outro menu, desta vez com mais opções, de 1 a 10, e caso queira retornar para o meu anterior, digite 99.

![image](https://github.com/user-attachments/assets/6ace947b-5e40-485a-9eb9-3e43fecf7d21)

 
- Vetor de ataque: agora escolheremos a opção 2) ``` Web Site Attack Vectors ``` e tecle enter.

![image](https://github.com/user-attachments/assets/1fb0a04a-fcbd-4edc-b4e1-b7709fb27bc6)

 
Na próxima tela aparecerá mais um menu, desta vez com menos opções, de 1 a 7, e caso queira retornar para o meu anterior, digite 99.
- Método de ataque: agora a nossa opção é a 3) ```Credential Harvester Attack Method ``` e teclamos enter.

 ![image](https://github.com/user-attachments/assets/5190a2f2-8772-4bd9-a017-456e85cf8698)

Na próxima tela aparecerá um menu, com apenas três opções, de 1 a 3, e caso queira retornar para o meu anterior, digite 99.
- Método de ataque: escolheremos a opção 2) ``` Site Cloner ``` e teclamos enter.

![image](https://github.com/user-attachments/assets/a6cbfbd5-0ff9-4ef1-b55a-bda91b382489)


Após digitar a opção 2) Site Cloner, precisaremos verificar o endereço IP da máquina do Kali Linux. 

- Sugestão: abra outro terminal e utilize o comando ``` ifconfig ```

![image](https://github.com/user-attachments/assets/b5794aa8-1fb7-4f4c-a993-1ba1dda03afe)


 
Aqui está o endereço IP que iremos utilizar. Digitamos ele e teclamos enter.
 ![image](https://github.com/user-attachments/assets/6fc89a55-20d3-4856-8508-38ecbbbc2292)

### OBS.: confira se é o mesmo IP que ele sugere, caso seja, basta dar um enter.
Agora entraremos com a página que será clonada, no nosso lab, será a do facebook.

 ![image](https://github.com/user-attachments/assets/81ce4799-e564-4ccf-9244-cb68dbf0b536)

URL para clone: http://www.facebook.com, após clicamos enter, ficará assim:
![image](https://github.com/user-attachments/assets/cb1927dc-2d4b-466c-bfe9-5c3b04a692b5)

 
Após teclado enter, ele construirá toda a estrutura para nosso acesso:
 ![image](https://github.com/user-attachments/assets/dfdf4744-d092-4273-beaf-c5df295eee55)

Para acessar, basta digitar o mesmo endereço IP utilizado na página clone, no nosso lab foi o 192.168.0.22, no seu navegador, em outra máquina que tenha acesso a esta máquina do lab.
 
![image](https://github.com/user-attachments/assets/02403935-0cb1-4dc5-aa3e-30a8782e2fc8)

Acessando via Edge, da máquina virtual com o Sistema Operacional Windows 7.
Na máquina do Kali Linux, a ferramenta começa a gerar vários reports:

![image](https://github.com/user-attachments/assets/5214394f-8a77-486e-a8f0-cc6b399f9162)

Agora é só aguardar o usuário entrar com login e senha para capturarmos.

![image](https://github.com/user-attachments/assets/4c00f9d3-2bea-4e92-8bbd-31cdf55c495c)

Está aí o resultado, email e senha capturados.

Laboratório Realizado com Sucesso!
