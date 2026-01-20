# Trabalho-de-Computação Gráfica, Alunos: Italo Francisco Almeida de Oliveira e Paulo Eduardo Lima Rabelo 


Trabalho da P3 da cadeira de Computação Gráfíca:

34. Aplicativo de AR para Plantas de Interiores
Descrição: Ajuda os usuários a visualizar como diferentes tipos de plantas ficariam em suas casas ou escritórios.


baixe o arquivo .apk em Releases, e instale no seu celular Angroid.
caso o arquivo .apk não funcione, siga o passo a passo abaixo:

Passo 1: Preparar o Ambiente (Unity)

Se você nunca usou Unity, precisará instalar as ferramentas corretas:

    Baixe e instale o Unity Hub.

    No Unity Hub, vá em Installs > Install Editor.

    Escolha uma versão recomendada (LTS, ex: 2021.3 ou 2022.3).

    Importante: Durante a instalação, marque a opção Android Build Support (e também os sub-itens OpenJDK e Android SDK & NDK Tools). Sem isso, você não consegue criar o app para celular.

Passo 2: Baixar o Projeto

    Clique no botão verde Code e depois em Download ZIP.

    Extraia (descompacte) a pasta em algum lugar do seu computador.

Passo 3: Abrir e Configurar no Unity

    Abra o Unity Hub, clique em Add e selecione a pasta que você extraiu.

    Abra o projeto (pode demorar um pouco na primeira vez).

    Com o projeto aberto, vá no menu superior: File > Build Settings.

    Na lista de "Platform", selecione Android e clique no botão Switch Platform (isso pode demorar uns minutos).

Passo 4: Ajustes Obrigatórios para AR (Realidade Aumentada)

Projetos de AR costumam dar erro se não configurados corretamente. Faça esta checagem rápida:

    Ainda na janela Build Settings, clique em Player Settings (canto inferior esquerdo).

    Vá na aba Player > Other Settings.

    Encontre a seção Graphics APIs. Se ver "Vulkan" na lista, clique nele e aperte o botão menos (-) para remover. (O ARCore do Google muitas vezes trava com Vulkan).

    Role para baixo até Minimum API Level e certifique-se de que está pelo menos no Android 7.0 'Nougat' (API Level 24) ou superior.

    Vá na aba XR Plug-in Management (no menu da esquerda) e garanta que a opção ARCore está marcada na aba de Android (ícone do robô).

Passo 5: Instalar no Celular

    No seu celular, ative o Modo Desenvolvedor:

        Vá em Configurações > Sobre o telefone.

        Toque 7 vezes em "Número da Versão" (Build Number).

    Entre nas Opções do Desenvolvedor e ative a Depuração USB (USB Debugging).

    Conecte o celular ao PC com o cabo USB.

    Volte ao Unity, na janela Build Settings.

    Em "Run Device", selecione o seu celular (se não aparecer, clique em Refresh).

    Clique em Build and Run.

    O Unity vai pedir para salvar o arquivo .apk (pode escolher qualquer pasta) e começará a compilar. Se der tudo certo, o app abrirá automaticamente no seu celular.
