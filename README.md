# OpenRGB-Artemis-2-Guia
Nesse guia vou descrever como fazer o OpenRGB e o ArtemisRGB trabalharem juntos. De Maneira que após a configuração seu único trabalho será abrir os dois programas para fazer seus efeitos RGB funcionarem.

IMPORTANTE:
Ambos os programas funcionam utilizando a tecnologia aRGB (Led Endereçável ou Addressable RGB) portanto antes de prosseguir verifique se suas peças são compatíveis com essa tecnologia, caso suas peças tenham suporte aos programas Asus AuraSync, RGB Fusion, iCUE, Razer Chroma, há grandes chances de possuir os LEDs aRGB, porém caso você esteja querendo montar um setup inteiro com peças aRGB sempre verifique antes, veja vídeos de pessoas que já possuem a peça para confirmar se os LEDs são de fato endereçáveis. Outra maneira de identificar é verificar se a sua peça possui a conexão aRGB da imagem abaixo.

<img width="304" height="163" alt="image" src="https://github.com/user-attachments/assets/a1038d1c-77c9-43ea-8527-d761986187ed" />

Também pode ocorrer de suas peças terem a conexão mas a sua placa mãe não, nesse caso recomendo fortemente que comprem a "Controladora RGB Nollie", a quantidade de canais vai depender de quantas peças você possui com essa tecnologia, indo entre 8, 16 ou 32 canais

- PRIMEIROS PASSOS

Você vai precisar de ambos os programas, OpenRGB e ArtemisRGB faça o download de acordo com a sua plataforma. (Windows, Linux, MacOS)

- OpenRGB: https://openrgb.org/

Após baixar o OpenRGB, ainda no site clique nos 3 traços do canto superior direito "Menu", vá em "Plugins", desça a página e vá até o OpenRGB Visual Map Plugin clique em "More Info and Releases"
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

- ArtemisRGB: https://artemis-rgb.com/

2 - Instalação do ArtemisRGB

2.1 - Tela inicial do instalador do Artemis.
![Artemis Imagem 1](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/Artemisimage1.png?raw=true)

2.2 - Caso você deseje trocar o local de instalação clique nas 3 bolinhas indicadas na imagem. (LEMBRE-SE DO LUGAR EM QUE FOI INSTALADO)
![Artemis Imagem 2](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/Artemisimage2.png?raw=true)

2.3 - Aguarde a instalação ser concluída.
![Artemis Imagem 3](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/Artemisimage3.png?raw=true)

2.4 - Desmarque a opção "Launch Artemis" e clique em "Finish".
![Artemis Imagem 4](https://github.com/ZaharDIO/OpenRGB-Artemis-2/blob/main/images/Artemisimage4.png?raw=true)

- Configurações iniciais

- 3 - OpenRGB

3.1 - Antes de iniciar o OpenRGB pela primeira vez, clique com o botão direito vá em propriedades e marque para sempre executar como administrador.

3.2 - Após abrir ignore tudo que estiver na sua tela e vá direto em Settings -> General Settings.

3.3 - Marque as caixas "Show LED View by Default", "Shared SMBus Access" e "Serve All Devices". (Se voce tiver uma CPU da AMD marque também a caixa "AMD SMBus")
![alt text](images/image-0.png)

3.4 - Ainda em Settings clique em Plugins -> Install Plugin
![alt text](images/image-1.png).

Escolha o arquivo OpenRGBVisualMapPlugin.dll baixado anteriormente.
![alt text](images/image-2.png)

Verifique se a caixa Enabled esta ativa, caso não esteja ative. 
![alt text](images/image-3.png)

3.5 - Clique em Save Profile, encerre o OpenRGB e abra novamente. 
![alt text](images/image-4.png)
              
- 4 - Visual Map 

4.1 - Após os passos anteriores o seu OpenRGB agora deve conter um botão adicional no topo escrito "Visual Map", nesse menu você montará o layout de LED das suas peças, ou seja, caso sua peça seja uma barra de LED Horizontal com 10 LEDs, você conseguirá identificar cada LED individual da sua barra, colocá-los na horizontal e ordená-los, tudo isso será ensinado nos passos a seguir.

4.2 - No Menu Lateral Esquerdo você encontrará todas as peças que o OpenRGB está reconhecendo no seu computador, por questões de representação do tamanho real das peças após a integração com o Artemis, recomendo que seja criado um Layout diferente para cada peça, mesmo sendo possível a criação de um Layout em que todas as peças estão juntas, isso cria vários problemas no futuro, então adicione apenas uma peça de sua escolha ao Layout.

Você pode criar um novo Layout clicando no Menu Lateral Esquerdo em "VMap", "New Map".
![alt text](images/image-6.png)

Adicione sua nova peça clicando no símbolo "+" ao lado da peça de sua escolha, caso te facilite a se localizar você pode renomear o nome da peça clicando no ícone do meio à esquerda do símbolo "+". 
![alt text](images/image-5.png)

Clique em "Auto Resize" no Menu Lateral Direito, e para desbugar sua visão vá ao Menu Lateral Direito em "Width" e "Height" coloque o valor de 20. 
![alt text](images/image-7.png)

Esse é o espaço em que você trabalhará com seus LEDs, caso sua peça tenha mais do que 20 LEDs de Largura aumente o "Width", 20 LEDs de Altura aumente o "Height", e assim por diante, não se preocupe muito com esses valores pois após o fim da configuração você usará o botão "Auto Resize" para deixar a peça no tamanho perfeito, mas para fazer a configuração recomendo que deixe um espaço amplo para nenhum LED ficar de fora do Grid.

4.3 - Clique na peça dentro do Grid e aperte o botão "Identify" no Menu Lateral Direito. 
![alt text](images/image-8.png)

Esse botão faz a peça acender na cor verde, assim facilitando a identificação da peça em que você está mexendo. 
![alt text](images/image-9.png)
![alt text](images/image-10.png)

4.4 - Ainda no Menu Lateral Direito clique no botão ao lado da palavra "Shape", escolha a opção "Custom"
Com isso surgirá um novo botão "Edit Shape".
![alt text](images/image-12.png) 

4.5 - Ao clicar em "Edit Shape" aparecerá o menu de configuração das posições dos LEDs da sua peça, nesse menu você tem várias opções para reordenar os LEDs, porém recomendo que teste por conta própria o que cada uma faz, por hora utilizaremos apenas o botão "Auto Identify" e reordenaremos manualmente, ao marcar essa opção você pode clicar em um LED de sua escolha e ele acenderá, assim você consegue definir exatamente qual a posição de cada LED de acordo com a sua peça.
![alt text](images/image-11.png)![alt text](images/image-13.png)
![alt text](images/image-14.png)![alt text](images/image-15.png)

Ao identificar as posições dos seus LEDs clique e arraste-os de maneira que eles fiquem na posição em que você acredite se encaixar melhor com a orientação das suas peças no gabinete. Caso precise aumentar o grid, mexa nas opções "Width" e "Height", assim como no Menu anterior é sempre importante deixar todos os LEDs dentro do Grid e apertar a opção Auto Resize ao final da configuração para garantir que a sua peça esta no tamanho correto. Ao finalizar clique em "Save".
![alt text](images/image-16.png)

4.6 - Quando terminar de configurar a sua peça no Menu Lateral Direito clique em "Auto Resize" e ele fechará o Grid no tamanho perfeito para a sua peça. Marque as caixas "Auto Load" e "Auto Register", clique em "VMap Menu", marque a opção "Register Controller" e clique em "Save", coloque o nome da sua peça, vá ao Menu Superior vá em "Devices" e clique em "Save Profile" para garantir que suas alterações foram salvas.
![alt text](images/image-17.png)
![alt text](images/image-18.png)
              
4.7 - Caso queira adicionar uma nova peça, repita os passos 4.2 em diante, até ter todas as suas peças mapeadas.

4.8 - Após finalizar a configuração dos seus layouts, vá ao Menu Inferior clique em Save Profile, no Menu Superior clique em "SDK Server", e depois em "Start Server".
![alt text](images/image-19.png)

- 5 - ArtemisRGB

5.1 - Ao abrir o ArtemisRGB, clique em "Continue" ao aparecer a aba de "Device Provider" vá até o plugin "OpenRGB Device Provider" e clique em "Enable Feature"

5.2 - Não marque nada e clique em "Continue" e depois "Finish", após isso vá em "Settings", desça até encontrar a opção "Target Frame Rate", coloque em 45 fps, após isso reinicie o seu ArtemisRGB, e o setup inicial está configurado.

5.3 - No ArtemisRGB você conseguirá configurar os efeitos de milhares de jeitos, ensinarei a fazer três efeitos diferentes: Ambilight, Rainbow e XInput.

5.4 - Antes de iniciar a criação dos efeitos é necessário verificar se o Layout do OpenRGB está chegando corretamente, para fazer isso clique em "Surface Editor" aqui você encontrará todas as suas peças. clique com o botão direito e depois em "Identify", esse botão fará sua peça começar a piscar, clique com o direito e vá em "View Properties" e depois em "Scale", esse parâmetro define a escala da sua peça, ajuste valores de acordo com a sua escolha para representar o tamanho real, pois você pode ter uma peça com 12 LEDs e 20cm, e uma com 12 LEDs e 10cm, como a escala inicial considera o valor 1, ambas as peças teriam o mesmo tamanho no "Surface Editor", o que resulta em efeitos aparecendo incorretamente, por isso é importante alterar a escala das suas peças para corresponder ao tamanho e posição delas em comparação com as outras no gabinete.

5.3 - Configuração de Efeitos
      
