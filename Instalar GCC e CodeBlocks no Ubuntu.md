
Instalar GCC e Code::Blocks no Ubuntu para compilar C++
===============================================

--------------------

## Antes de tudo, atualizar os repositórios e gatilhos do Ubuntu:

> sudo apt-get update

> sudo apt-get upgrade


## Instalando o GCC:

1. Abra o terminal e digite os seguintes comandos:

	> sudo apt-get update 		*// Atualizar o repositório*
	
	> sudo apt-get upgrade	   	*// Instalar as atualizações no repositório*
	
	> sudo apt-get install g++	*// Instalar a ultima versão estável do compilador do C++*

	- No momento a distribuição padrão do Ubuntu Linux inclui um compilador GNU C, mas não inclui as extensões de C++.

2. Digite o seguinte comando no terminal:

	> gcc-version
	
	- *Comando para saber a versão atual do GCC. A cima de 4.7.1 já está bom.*

3. Se você estiver usando Debian Linux, os comandos são os mesmos. Se você estiver usando o Red Hat Linux, substitua o comando apt-get pelo yum, ficando: 

	> sudo yum install g++


## Instalando o Code::Blocks:

1. Abrar o terminal e digite:

	> sudo apt-get install codeblocks
	
	- *Comando para instalar o Code::Blocks*

2. Abra o Code::Blocks, vá em "Settings> Compiler". Marque as opções:

	- **Enable all common compiler warnings (overrides many other settings)**

	- **Have g++ follow the coming C++0x ISO C++ language standard**

	- **Have g++ follow the C++11 ISO C++ language standard**

3. Selecione a aba **"Toolchain Executables"** e clique no botão **"..."** Navegue até a pasta **"/usr"**, à menos que você tenha instalado em outro diretório que não seja **"/user/bin"**.

4. Nas seguintes opções deixe como especificado a baixo:

	- C Compiler => deve ser **gcc**

	- C++ Compiler => deve ser **g++**
		
	- Linker for dynamic libs => deve ser **g++**

5. Efetuadas as alterações selecione **OK** para salvar e finalizar as configurações.

--------------------

## Fontes

http://www.dummies.com/how-to/content/how-to-install-c-codeblocks-in-ubuntu-linux.html
