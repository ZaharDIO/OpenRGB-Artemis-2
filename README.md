# OpenRGB-Artemis-2-Guia
Nesse guia vou descrever como fazer o OpenRGB e o ArtemisRGB trabalharem juntos.

IMPORTANTE:
Ambos os programas funcionam utilizando a tecnologia aRGB (Led Endereçável ou Addressable RGB) portanto antes de prosseguir verifique se suas peças são compatíveis com essa tecnologia, caso suas peças tenham suporte aos programas Asus AuraSync, RGB Fusion, iCUE, há grandes chances de possuir os LEDs aRGB, porém caso voce esteja querendo montar um setup inteiro com peças aRGB sempre verifique antes, veja vídeos de pessoas que já possuem a peça para confirmar se os LEDs são de fato endereçáveis. Outra maneira de identificar é verificar se a sua peça possui a conexão aRGB da imagem abaixo.

<img width="304" height="163" alt="image" src="https://github.com/user-attachments/assets/a1038d1c-77c9-43ea-8527-d761986187ed" />


PRIMEIROS PASSOS

Você vai precisar de ambos os programas, OpenRGB e Artemis 2 faça o download de acordo com a sua plataforma. (Windows, Linux, MacOS)

- OpenRGB: https://openrgb.org/

Após baixar o OpenRGB, clique nos 3 traços do canto superior direito "Menu", vá em "Plugins", desça a página e vá até o OpenRGB Visual Map Plugin clique em "More Info and Releases"
Baixe a versão de acordo com sua plataforma, e salve em um local em que voce se lembrará. (Caso seja WINDOWS: Baixe a versão Windows (64-bit), não baixe a versão installer)

1 - Instalação do OpenRGB
1.1 - Após baixar o instalador abra e siga os passos de instalação conforme as imagens a seguir.

1.2 - Clique em "Next" para prosseguir com a instalação.
![OpenRGB Imagem 1](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/imagem1.png?raw=true)

1.3 - Aceite os termos de uso e clique em "Next".
![OpenRGB Imagem 2](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/imagem2.png?raw=true)

1.4 - Caso você deseje trocar o local de instalação clique em "Change" e siga os passos 1.4.1 em diante. (LEMBRE-SE DO LUGAR EM QUE FOI INSTALADO POIS O MESMO SERÁ NECESSÁRIO NO FUTURO)
![OpenRGB Imagem 3](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/imagem3.png?raw=true)

1.4.1 - Selecione o local de instalação desejado.
![OpenRGB Imagem 4](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/imagem4.png?raw=true)

1.4.2 - Confirme o local de instalação

![OpenRGB Imagem 5](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/imagem5.png?raw=true)

1.5 - Nessa tela clique em "Install System Service", e confirme com "Sim".
![OpenRGB Imagem 6](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/imagem6.png?raw=true)

- Artemis 2: https://artemis-rgb.com/

2 - Instalação do Artemis 2

2.1 - Tela inicial do instalador do Artemis.
![Artemis Imagem 1](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/Artemisimage1.png?raw=true)

2.2 - Caso você deseje trocar o local de instalação clique nas 3 bolinhas indicadas na imagem. (LEMBRE-SE DO LUGAR EM QUE FOI INSTALADO)
![Artemis Imagem 2](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/Artemisimage2.png?raw=true)

2.3 - Aguarde a instalação ser concluída.
![Artemis Imagem 3](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/Artemisimage3.png?raw=true)

2.4 - Desmarque a opção "Launch Artemis" e clique em "Finish".
![Artemis Imagem 4](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/Artemisimage4.png?raw=true)

- Configurações iniciais

3 - OpenRGB

3.1 - Antes de iniciar o OpenRGB pela primeira vez, clique com o botão direito vá em propriedades e marque para sempre executar como administrador. (IMAGENS)

3.2 - Após abrir ignore tudo que estiver na sua tela e vá direto em Settings -> General Settings. (IMAGEM)

3.3 - Marque as caixas "Show LED View by Default", "Shared SMBus Access" e "Serve All Devices". (Se voce tiver uma CPU da AMD marque também a caixa "AMD SMBus") (IMAGEM)

3.4 - Ainda em Settings clique em Plugins -> Install Plugin, e escolha o arquivo OpenRGBVisualMapPlugin.dll baixado anteriormente. Verifique se a caixa Enabled esta ativa, caso não esteja ative. (IMAGENS)

3.5 - Clique em Save Profile, encerre o OpenRGB e abra novamente. (IMAGEM)
              
4 - Visual Map 

4.1 - Após os passos anteriores o seu OpenRGB agora deve conter um botão adicional no topo escrito "Visual Map", (IMAGEM) nesse menu você montará o layout de LED das suas peças, ou seja, caso sua peça seja uma barra de LED Horizontal com 10 LEDs, você conseguirá identificar cada LED individual da sua barra, colocá-los na horizontal e ordená-los, tudo isso será ensinado nos passos a seguir.

4.2 - No Menu Lateral Esquerdo você encontrará todas as peças que o OpenRGB está reconhecendo no seu computador, (IMAGEM DO MENU LATERAL) por questões de representação do tamanho real das peças após a integração com o Artemis, recomendo que seja criado um Layout diferente para cada peça, mesmo sendo possível a criação de um Layout em que todas as peças estão juntas, isso cria vários problemas no futuro, então adicione apenas uma peça de sua escolha ao Layout clicando no símbolo "+" ao lado da peça de sua escolha, caso te facilite a se localizar você pode renomear o nome da peça clicando no ícone do meio à esquerda do símbolo "+". (IMAGEM DO RENAME E DO +)

4.3 - Ao adicionar a peça ao Grid, vá ao Menu Lateral Direito em "Width" e "Height" coloque o valor de 20, (IMAGEM) esse é o espaço em que você trabalhará com seus LEDs, caso sua peça tenha mais do que 20 LEDs de Largura aumente o "Width", 20 LEDs de Altura aumente o "Height", e assim por diante, não se preocupe muito com esses valores pois após o fim da configuração você usará o botão "Auto Resize" para deixar a peça no tamanho perfeito, mas para fazer a configuração recomendo que deixe um espaço amplo para nenhum LED ficar de fora do Grid.

4.4 - Clique na peça dentro do Grid e aperte o botão "Identify" no Menu Lateral Direito, (IMAGEM) esse botão faz a peça acender na cor verde, assim facilitando a identificação da peça em que você está mexendo. (IMAGEM DA PEÇA ACESA)

4.5 - Ainda no Menu Lateral Direito clique no botão ao lado da palavra "Shape", escolha a opção "Custom", com isso surgirá um novo botão "Edit Shape". (IMAGENS)

4.6 - Ao clicar em "Edit Shape" aparecerá o menu de configuração das posições dos LEDs da sua peça, Nesse menu você tem várias opções para reordenar os LEDs, porém recomendo que teste por conta própria o que cada uma faz, por hora utilizaremos apenas o botão "Auto Identify" e reordenaremos manualmente, ao marcar essa opção você pode clicar em um LED de sua escolha e ele acenderá, assim você consegue definir exatamente qual a posição de cada LED de acordo com a sua peça. (NESSA PARTE EU TENHO QUE MOSTRAR EXEMPLOS COM A MINHA BARRA DE LED VERTICAL ACENDENDO O LED 1 POR 1) Ao identificar as posições dos seus LEDs clique e arraste-os de maneira que eles fiquem na posição em que você acredite se encaixar melhor com a orientação das suas peças no gabinete. Ao finalizar clique em "Save".

4.7 - Quando terminar de configurar a sua peça clique em "Auto Resize" e ele fechará o Grid no tamanho perfeito para a sua peça. No Menu Lateral Direito marque as caixas "Auto Load" e "Auto Register", clique em "VMap Menu", marque a opção "Register Controller" e clique em "Save", coloque o nome da sua peça, vá ao Menu Superior vá em "Devices" e clique em "Save Profile" para garantir que suas alterações foram salvas.
              
4.8 - Caso queira adicionar uma nova peça, volte ao menu "Visual Map", no Menu Lateral Esquerdo clique em "VMap", "New Map", Adicione sua nova peça clique em "Auto Resize" para desbugar sua visão e aumente o tamanho do Grid novamente ("Width" e "Height"), repita os passos 4.2 em diante para definir o Layout da sua peça novamente, e vá fazendo isso até ter todas as suas peças mapeadas em Layouts diferentes
      
