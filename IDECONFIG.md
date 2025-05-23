# 📃 | Ambientação

Para a ambientação do projeto foi utilizado o Visual Studio Code (VSCode) junto a extensão da Espressif disponibilizada no VSCode, já que a programação da plataforma ESP RainMaker recebe mais suporte via ESP-IDF. Com isso, segue a instalação e configuração das ferramentas utilizadas:

## ⚠️ | Observações:
  
- As ferramentas foram utilizadas no sistema operacional Windows (mais especificamente no Windows 11) nas versões disponíveis entre os meses de Março e Junho de 2025
- Nenhum dos diretórios deve ter caracteres especiais
- Os itens necessários para o funcionamento integral das ferramentas devem ser intrinsicamente instalados/colocados nas pastas indicadas

Desse modo, o funcionamento do projeto é garantido tendo em vista as restrições acima em vigência no período de desenvolvimento citado

## 0. Instalação do ESP-IDF 

Primeiramente, é necessário baixar o ESP-IDF pelo link https://dl.espressif.com/dl/esp-idf/ (utilizar preferencialmente o instalador online):
 
<p align = center>
  <img src = "img/ESP-IDF_DOWNLOAD.png">
</p>
  
Na instalação, selecione o diretório de instalação como o seu **Disco Local (C:)**

## 1. Instalar o VSCode 

  A instalação da IDE não segue um criterio especifico para o seu funcionamento posteriormente. Assim, você pode simplesmente baixar pelo site: (https://code.visualstudio.com) a IDE e depois instalar onde achar oportuno.

## 2. Instalação da extensão na IDE 

- Na aba **Extensions** do VSCode, procurar por **ESP-IDF** e instalar;

<p align = center>
  <img src = "img/EXTENSAO_VSCODE.png">
</p>

- Depois de instalar, uma aba de configuração deve aparecer. Caso não aconteça, busque por **>Configure ESP-IDF Extension** na barra de pesquisa da IDE localizada no centro da barra superior da interface.

  <p align = center>
    <img src = "img/CONFIGURE_IDE.png">
  </p>


  ### Atenção nas proximas instruções! ⚠️  

  Agora na aba de configuração:

- Selecione a opção **Advanced**;

  <p align = center>
    <img src = "img/MENU_EXTENSION_CONFIG.png">
  </p>

- Os itens que devem aparecer são estes:

  <p align = center>
    <img src = "img/MENU_EXTENSION_CONFIG_PATH.png">
  </p>

- Atribua a cada um deles os respectivos caminhos e clique em **Configure Tools**. Os caminhos ser iguais ao da imagem considerando que os passos anteriores tenham sido cumpridos;

- Após isso, espera-se que um conjunto de ferramentas sejam instaladas no seu sistema e um icone apareça na barra no canto esquerdo da ide;
    
   <p align = center>
    <img src = "img/IDE_CONFIG_END.png">
  </p>
    
  Por fim, a sua IDE está pronta para utilizar as ferramentas de desenvolvimento padrão da espressif no projeto.
  
### Recomendação | ⏭️

  A espressif tem um diretorio no github onde eles disponibilizam ,junto a um tutorial de instalação, uma explicação de cada atalho da extensão que você pode acessar neste link para mais dúvidas https://github.com/espressif/vscode-esp-idf-extension/blob/master/README.md.

#

### Muita Atenção nas proximas instruções! ⚠️⚠️⚠️  

  Visando o funcionamento amplo do projeto, os arquivos disponibilizados para download foram configurados para buscar bibliotecas e itens importantes com base em variáveis de ambiente do sistema do seu computador. Sendo assim, qualquer descuido na configuração dessas variáveis e afins implica diretamente ao não funcionamento do projeto!
  
## 3. Configuração para desenvolvimento do ESPRainMaker

  #### Alocação de pastas
  
  - Neste repositório foi disponibilizado um zip do projeto chamado "RainMaker" para download (colocar aq o link), depois de descompactar pegue a pasta e coloque em : "C:\Espressif\frameworks\esp-idf-v5.4.1\examples";

  - Após isso, baixe o zip ["lib_sensors"](https://github.com/enzoaccioly1/projeto-integrador-I/raw/main/source/lib_sensors.rar), descompacte-o e pegue todas as pastas dentro da pasta de mesmo nome e coloque em: "C:\Espressif\frameworks\esp-idf-v5.4.1\components".

  #### Implementação das variáveis de ambiente

  - Acesse o menu de variáveis de ambiente via **win+r** e depois digite na aba que aparecer: **sysdm.cpl** ou pesquise na aba de pesquisa do windows. Posteriormente você vai poder visualizar as variaveis de sistema e usuário no seu computador;
  
   <p align = center>
    <img src = "img/VARIAVEIS_DE_AMBIENTE.png">
  </p>

  - Agora faça 2 variaveis de <ins>sistema</ins> com os nomes **IDF_PATH** e **RMAKER_PATH** e adicione os seus diretórios correspondentes como na imagem acima;
  - Aplique as suas alterações e reinicie o seu computador.

  Com isso, o projeto está pronto para ser executado.
  
