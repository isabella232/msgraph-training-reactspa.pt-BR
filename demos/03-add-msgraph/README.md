# <a name="how-to-run-the-completed-project"></a>Como executar o projeto concluído

## <a name="prerequisites"></a>Pré-requisitos

Para executar o projeto concluído nessa pasta, você precisará do seguinte:

- [Visual Studio](https://visualstudio.microsoft.com/vs/) instalado em sua máquina de desenvolvimento. Se você não tiver o Visual Studio, visite o link anterior para opções de download. (**Observação:** este tutorial foi escrito com o Visual Studio 2017 versão 15,81. As etapas deste guia podem funcionar com outras versões, mas que não foram testadas.
- Uma conta pessoal da Microsoft com uma caixa de correio no Outlook.com ou uma conta corporativa ou de estudante da Microsoft.

Se você não tem uma conta da Microsoft, há algumas opções para obter uma conta gratuita:

- Você pode [se inscrever para uma nova conta pessoal da Microsoft](https://signup.live.com/signup?wa=wsignin1.0&rpsnv=12&ct=1454618383&rver=6.4.6456.0&wp=MBI_SSL_SHARED&wreply=https://mail.live.com/default.aspx&id=64855&cbcxt=mai&bk=1454618383&uiflavor=web&uaid=b213a65b4fdc484382b6622b3ecaa547&mkt=E-US&lc=1033&lic=1).
- Você pode [se inscrever no programa para desenvolvedores do office 365](https://developer.microsoft.com/office/dev-program) para obter uma assinatura gratuita do Office 365.

## <a name="register-a-web-application-with-the-application-registration-portal"></a>Registrar um aplicativo Web com o portal de registro do aplicativo

1. Abra um navegador e navegue até o [portal de registro do aplicativo](https://apps.dev.microsoft.com). Faça logon usando uma **conta pessoal** (aka: conta da Microsoft) ou **conta corporativa ou de estudante**.

1. Selecione **Adicionar um aplicativo** na parte superior da página.

    > **Observação:** Se você vir mais de um botão **Adicionar um aplicativo** na página, selecione aquele que corresponde à lista **aplicativos convergidos** .

1. Na página **registrar seu aplicativo** , defina o **nome do aplicativo** como o **tutorial de gráfico reagir** e selecione **criar**.

    ![Captura de tela da criação de um novo aplicativo no site do portal de registro de aplicativo](/tutorial/images/arp-create-app-01.png)

1. Na página enviar o **tutorial do gráfico de reagir** , na seção **Propriedades** , copie a **ID do aplicativo** , pois você precisará dela mais tarde.

    ![Captura de tela da ID do aplicativo recém-criado](/tutorial/images/arp-create-app-02.png)

1. Role para baixo até a seção **plataformas** .

    1. Selecione **Adicionar plataforma**.
    1. Na caixa de diálogo **Adicionar plataforma** , selecione **Web**.

        ![Captura de tela criando uma plataforma para o aplicativo](/tutorial/images/arp-create-app-03.png)

    1. Na caixa plataforma **da Web** , insira `http://localhost:3000` para as **URLs**de redirecionamento.

        ![Captura de tela da nova plataforma Web adicionada para o aplicativo](/tutorial/images/arp-create-app-04.png)

1. Role até a parte inferior da página e selecione **salvar**.

## <a name="configure-the-sample"></a>Configurar o exemplo

1. ReNomear `./graph-tutorial/src/Config.js.example` o `./graph-tutorial/src/Config.js`arquivo para.
1. Edite `./graph-tutorial/src/Config.js` o arquivo e faça as seguintes alterações.
    1. Substitua `YOUR_APP_ID_HERE` pela **ID do aplicativo** obtida do portal de registro do aplicativo.
1. Na sua interface de linha de comando (CLI), navegue até `graph-tutorial` o diretório e execute o comando a seguir para instalar os requisitos.

    ```Shell
    npm install
    ```

## <a name="run-the-sample"></a>Executar o exemplo

1. Execute o comando a seguir em sua CLI para iniciar o aplicativo.

    ```Shell
    npm start
    ```

1. Abra um navegador e navegue até `http://localhost:3000`.