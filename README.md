![Rocketseat](assets/rocketseat.png)

**Importante: todo o conteúdo do antigo PDF para configuração do ambiente de desenvolvimento foi migrado para este repositório. Dessa forma fica mais fácil manter todas as informações atualizadas e incluir ainda soluções para as dificuldades mais comuns que os devs encontram.**

# Ambiente React Native (Android/iOS)

Para testar nossas aplicações em dispositivos reais iremos utilizar emuladores que são apps que imitam o funcionamento de um dispositivo físico dentro do nosso sistema. Infelizmente no Windows e no Linux ainda não é possível configurar um emulador de iOS de forma nativa e, por isso, vamos focar no Android nessas duas plataformas.

## Editor

O editor de código que utilizo para construção das minhas apps mobile é o Visual Studio Code da Microsoft. Com ele tenho uma interface muito semelhante aos editores Sublime Text e Atom enquanto mantenho recursos como autocomplete, debugging e outras features presentes apenas em IDE's.

O VSCode não é obrigatório e você pode utilizar o que preferir. Dentre os que eu recomendo estão: VSCode, Sublime Text, Atom e Vim.

Snippets para VSCode: https://marketplace.visualstudio.com/items?itemName=rocketseat.RocketseatReactNative

## Android

Para termos um ambiente de desenvolvimento para Android iremos instalar a SDK do mesmo com ferramentas adicionais para executarmos nossa app em um emulador. Da mesma forma, ao fim desse guia você também poderá emular sua aplicação em seu dispositivo físico utilizando USB.

O ambiente Android pode ser configurado no Mac OSX, Linux e Windows, siga o guia abaixo de acordo com seu sistema operacional.

### Windows

1. Instale o Chocolatey e as demais dependências: [Instalando chocolatey](windows-chocolatey.md)
2. Instale a configure a SDK do Android: [Configurando SDK](windows-android-sdk.md)
3. Instale e configure o emulador Genymotion: [Configurando Genymotion](genymotion.md)

### Linux

1. Instale NodeJS, JDK e demais dependências: [Instalando dependências](linux-dependencias.md)
2. Instale a configure a SDK do Android: [Configurando SDK](unix-android-sdk.md)
3. Instale e configure o emulador Genymotion: [Configurando Genymotion](genymotion.md)


### OS X (Mac)

1. Instale NodeJS, JDK e demais dependências: [Instalando dependências](osx-dependencias.md)
2. Instale a configure a SDK do Android: [Configurando SDK](unix-android-sdk.md)
3. Instale e configure o emulador Genymotion: [Configurando Genymotion](genymotion.md)

## iOS (Apenas Mac)

Para configurar o ambiente de iOS no OS X basta ter instalado o XCode no sistema. Caso você ainda não tenha instalado, você pode baixar o mesmo pelo link https://developer.apple.com/xcode/

Com o XCode instalado, basta executar o seguinte comando na pasta de um projeto React Native para rodar o React Native no simulador de iOS:

```sh
react-native run-ios
```

Você pode ainda escolher a versão do emulador utilizado passando uma propriedade `--simulator`:

```sh
react-native run-ios --simulator="iPhone XS Max"
```

## Erros comuns

Para resolução de erros comuns no processo de configuração de ambiente do React Native, acesse [Erros comuns](erros-comuns.md)
