# Configurando SDK do Android no Windows

Crie uma pasta em um local desejado para instalação da SDK. Ex: `C:\Android\Sdk`.

*Anote esse caminho para ser utilizado posteriormente*

Acesse https://developer.android.com/studio/#downloads, na opção "Command line tools only" baixe a SDK referente ao seu sistema operacional.

Após feito o Download, extraia o conteúdo do pacote para a pasta criada no passo anterior.

Agora, no Painel de Controle do Windows, abra o item “Sistema e Segurança” ou “Sistema”, clique em “Configurações avançadas do sistema”, selecione “Variáveis de ambiente” e clique no botão “Nova variável de ambiente”, indique o nome da variável como ANDROID_HOME, adicione o caminho utilizado acima (Ex: C:\Android\Sdk) como segundo parâmetro e clique em OK.

![Variável ambiente](/assets/5.png)

Na mesma janela de "Variáveis de ambiente" no Windows, clique na variável PATH e então em "Editar". Haverá uma lista de caminhos e você deve adicionar esses dois novos caminhos no fim da lista:

```
%ANDROID_HOME%\platform-tools
%ANDROID_HOME%\tools
```

Agora, abra seu Command Prompt ou PowerShell como administrador e execute o seguinte comando:

```sh
C:\Android\Sdk\tools\bin\sdkmanager  "platform-tools" "platforms;android-27" "build-tools;27.0.3" 
```

*Aceite todas licensas digitando `y` quando necessário.
