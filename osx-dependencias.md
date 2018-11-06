Para configurar o ambiente Android no Linux, vamos precisar instalar 3 dependências: Node, Watchman, JDK. Para boa parte desses pacotes utilizaremos o Homebrew para instalação.

## Instalando Homebrew

O Homebrew é um gerenciador de pacotes para OS X muito famoso e útil. Vamos instalá-lo em nosso sistema como seguinte comando:

```sh
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

## Instalando Node e Watchman

Com o Homebrew instalado, vamos instalar o NodeJS e o Watchman:

```sh
brew install node
brew install watchman
```

## Instalando React Native CLI

Com o NodeJS instalado podemos seguir para a instalação do CLI (Command Line Interface) do React Native:

```sh
npm install -g react-native-cli

// Ou yarn global add react-native-cli
```

## Instalando JDK (Java Development Kit)

O último item a ser instalado é o JDK (Java Development Kit) do Java que pode ser baixado pelo link (Após instalado, execute o .dmg e instale seguindo os passos do instalador): http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
