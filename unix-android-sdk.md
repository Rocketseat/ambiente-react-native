# Configurando SDK do Android no Linux/OS X (Mac)

Crie uma pasta em um local desejado para instalação da SDK. Ex: `~/Android/Sdk`

*Anote esse caminho para ser utilizado posteriormente*

Acesse https://developer.android.com/studio/#downloads, na opção "Command line tools only" baixe a SDK referente ao seu sistema operacional.

Após feito o Download, extraia o conteúdo do pacote para a pasta criada no passo anterior.

Com esse endereço precisamos configurar algumas variáveis ambiente em nosso sistema, procure pelo primeiro dos seguintes arquivos existentes no seu sistema: `~/.bash_profile` , `~/.profile` ou `~/.zshrc` , e adicione essas três linhas no arquivo (de preferência no início):

```sh
export ANDROID_HOME=~/Android/Sdk
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/platform-tools
```

*Se nenhum desses arquivos existir, crie o `~/.bash_profile`.*
*Caso esteja utilizando uma pasta diferente para a SDK do Android, altere acima.*

Agora, abra seu Terminal e execute o seguinte comando:

```sh
~/Android/Sdk/tools/bin/sdkmanager  "platform-tools" "platforms;android-27" "build-tools;27.0.3" 
```

*Aceite todas licensas digitando `y` caso necessário.
