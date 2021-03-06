<h1 align="center">Instalar Java no Ubuntu</h1>

## Na linha de comando.

Abra o terminal e siga os seguintes passos:

- Atualize os repositórios e o sistema:

	> sudo apt update

	> sudo apt upgrade

- Inclua o repositório oficial do Java.

	> sudo add-apt-repository ppa:webupd8team/java

- Atualize o repositório.

	> sudo apt update

- *(OPCIONAL)* Pesquise as versões disponíveis do Java e instale a desejada. O comando vai listar as informações do pacote.

	> sudo apt-cache search java (ou jdk)


- Instale o Java.

	> sudo apt install oracle-java8-installer

- Dê *Ok* na opção que aparecerá e depois aceite os termos da licença.

	`Do you accept  the Oracle Binary Code license terms?`**`Yes`**
			

- Verifique se o java foi instalado corretamente. O comando verfica se o JRE foi mesmo instalado na máquina, mostrando as informações do java.

	> java -version

	- Exemplo de saída:

		`java version "1.8.0_121"`</br>
		`Java(TM) SE Runtime Environment (build 1.8.0_121-b13)`</br>
		`Java HotSpot(TM) 64-Bit Server VM (build 25.121-b13, mixed mode)`


- Verifique se o java foi configurado corretamente. O camando verfica se o compilador do Java funciona. Ao contrário do Windows que é preciso setar a Variável de Ambiente, no Ubuntu (Linux) não é preciso.

	> javac -version

	- Exemplo de saída:

		`javac 1.8.0_121`

## Referências

<https://www.youtube.com/watch?v=BTNp4P12DIs>

<https://www.digitalocean.com/community/tutorials/como-instalar-o-java-no-ubuntu-com-apt-get-pt>

<https://www.debian.org/doc/manuals/apt-howto/ch-search.pt-br.html>

