# OpenRGB-Artemis-2-Guia
Nesse guia vou descrever como fazer o OpenRGB e o ArtemisRGB funcionarem juntos

IMPORTANTE
Ambos os programas funcionam utilizando a tecnologia aRGB (Led Endereçável ou Addressable RGB) portanto antes de prosseguir verifique se suas peças são compatíveis com essa tecnologia, caso suas peças tenham suporte aos programas Asus AuraSync, RGB Fusion, iCUE, ha grandes chances de ele possuir os Leds aRGB, porem caso voce esteja querendo montar um setup inteiro com peças aRGB sempre verifique antes se os Leds de fato são endereçáveis. Outra maneira de identificar e verificar se sua peça possui o cabo aRGB da imagem abaixo, porem sempre confirme, veja videos de pessoas que ja possuem a peça para verificar se os Leds são de fato compatíveis.

Primeiros passos
Você vai precisar de ambos os programas, baixe os de acordo com sua plataforma (Windows, Linux, MacOS)

1 - OpenRGB: https://openrgb.org/
Apos baixar o OpenRGB, clique nos 3 traços do canto superior direito "Menu", va em "Plugins" desça a pagina e va ate o OpenRGB Visual Map Plugin clique em "More Info and Releases"
Baixe a versão de acordo com sua plataforma, e salve em um local em que voce se lembrara (Caso seja Windows baixe a versão Windows (64-bit), não baixe a versão installer)

1.1 - Instalação do OpenRGB
1.11 - Apos baixar o instalador abra e siga os passos de Instalação conforme as imagens a seguir

1.12 - Clique em Next para prosseguir com a instalação
![OpenRGB Imagem 1](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/imagem1.png?raw=true)

1.13 - Aceite os termos de uso e clique em Next
![OpenRGB Imagem 2](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/imagem2.png?raw=true)

1.14 - Caso voce deseje trocar o local de instalação clique em "Change" e siga os passos 1.14.1 em diante (LEMBRE-SE DO LUGAR EM QUE FOI INSTALADO POIS O MESMO SERA NECESSÁRIO EM UM PASSO FUTURO)
![OpenRGB Imagem 3](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/imagem3.png?raw=true)

1.14.1 - Selecione o local de instalação desejado
![OpenRGB Imagem 4](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/imagem4.png?raw=true)

1.14.2 - Confirme o local de instalação

![OpenRGB Imagem 5](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/imagem5.png?raw=true)

1.15 - Na tela de Install System Service, clique em Install e confirme com Sim
![OpenRGB Imagem 6](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/imagem6.png?raw=true)

2 - Artemis: https://artemis-rgb.com/

2.1 - Instalação

2.11 - Tela inicial do instalador do Artemis
![Artemis Imagem 1](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/Artemisimage1.png?raw=true)

2.12 - Caso voce deseje trocar o local de instalação clique nas 3 bolinhas indicadas na imagem (LEMBRE-SE DO LUGAR EM QUE FOI INSTALADO)
![Artemis Imagem 2](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/Artemisimage2.png?raw=true)

2.13 - Aguarde a instalação ser concluída
![Artemis Imagem 3](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/Artemisimage3.png?raw=true)

2.14 - Instalação concluída com sucesso
![Artemis Imagem 4](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/Artemisimage4.png?raw=true)

3 - Configuração OpenRGB

3.1 - OpenRGB
3.11 - Antes de iniciar o OpenRGB pela primeira vez, clique com o botão direito va em propriedades e marque para sempre executar como administrador
3.12 - Apos abrir ignore tudo que estiver na sua tela e va direto em Settings -> General Settings
3.13 - Marque as caixas "Minimize on Close", "Show LED View by Default", Shared SMBus Access, e Serve All Devices,(Se voce tiver uma CPU da AMD marque também a caixa "AMD SMBus")
3.14 - Ainda em Settings clique em Plugins -> Install Plugin, e escolha o arquivo OpenRGBVisualMapPlugin.dll baixado anteriormente. Verifique se a caixa Enabled esta ativa, caso não esteja ative.
3.15 - Clique em Save Profile, encerre o OpenRGB e abra novamente
              
        3.2 - Visual Map 
3.21 - Apos os passos anteriores o seu OpenRGB agora deve conter um botão adicional no topo escrito "Visual Map", nesse menu voce montara o layout de Led das suas peças, ou seja, caso sua peça seja uma barra de Led Horizontal com 10 Leds, voce conseguira identificar cada Led individual da sua barra, coloca-los na horizontal e ordenados tudo isso sera ensinado nos passos a seguir.
              3.22 - No Menu Lateral Esquerdo voce encontrara todas as peças que o OpenRGB esta reconhecendo no seu computador, por questões de representação do tamanho real das peças e integração com o Artemis recomendo que crie um Layout para cada peça, mesmo sendo possível a criação de um Layout em que todas as peças estão juntas isso cria vários problemas no futuro, então adicione apenas uma peça de sua escolha ao layout clicando no simbolo + ao lado da peça de sua escolha, caso facilite para sua localização voce pode renomear o nome da peça clicando no ícone do meio a esquerda do +
              3.23 - Ao adicionar a peça ao Grid, va ao Menu Lateral Direito em Width e Height coloque o valor de 20, esse e o espaço em que voce trabalhara com seus Leds, caso sua peça tenha mais do que 20 Leds de Largura aumente o Width, 20 Leds de Altura aumente o Height, e assim por diante, não se preocupe muito com esses valores pois apos o fim da configuração voce usara o botão Auto Resize para deixar a peça no tamanho perfeito, porem para fazer a configuração recomendo que deixe um espaço amplo para nenhum LED ficar de fora do Grid.
              3.24 - Clique na peça dentro do Grid e aperte o botão Identify no Menu Lateral Direito, esse botão faz a peça acender na cor verde, assim facilitando a identificação da peça em que voce esta mexendo
              3.25 - Apos identificado ainda no Menu Lateral Direito clique no botão ao lado da palavra "Shape", escolha a opção Custom, apos isso surgira um novo botão Edit Shape
              3.26 - Ao clicar em Edit Shape aparecera o menu de configuração das posições dos LEDs da sua peça, Nesse menu voce tem varias opções para reordenar os Leds porem recomendo que teste por conta própria o que cada uma faz, por hora utilizaremos apenas o Auto Identify, ao marcar essa opção voce pode clicar no LED individualmente e ele acendera, assim voce consegue definir exatamente qual a posição de cada LED em seu grid, (NESSA PARTE EU TENHO QUE MOSTRAR EXEMPLOS COM A MINHA BARRA DE LED VERTICAL ACENDENDO O LED 1 POR 1). Ao identificar as posições dos seus LEDS clique e arraste os de maneira que eles fiquem na posição em que voce acredite se encaixar melhor de acordo com a orientação das suas peças no Gabinete. Ao Finalizar clique em Save.
              3.27 - Quando terminar de configurar a sua peça clique em Auto Resize e ele fechara o Grid no tamanho perfeito para a sua peça, no Menu Lateral Esquerdo Marque as caixas Auto Load e Auto Register, clique em VMap Menu, marque a opção Register Controller e clique em Save, Coloque o nome da sua Peça, No Menu Superior volte em Devices e clique em Save Profile para garantir que suas alterações foram salvas
              3.28 - Caso queira adicionar uma nova peça, volte ao menu Visual Map, no Menu Lateral Esquerdo clique em VMap, New Map, Adicione sua nova peça clique em Auto Resize para desbugar sua visão e aumente o tamanho do Grid novamente, repita os passos anteriores para definir o Layout da sua peça novamente, e va fazendo isso ate ter todas as suas peças mapeadas
      
