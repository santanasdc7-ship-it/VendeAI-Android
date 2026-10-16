# VendeAI para Android — projeto que gera APK

Este pacote contém um projeto Android Studio que empacota a interface existente do VendeAI num aplicativo Android (WebView), e uma automação GitHub Actions para compilar o APK sem instalar ferramentas no celular.

## Gerar o APK usando apenas o celular
1. Entre/crie uma conta em https://github.com/.
2. Crie um repositório novo chamado `VendeAI-Android`.
3. Envie os arquivos deste ZIP para o repositório, preservando as pastas e o caminho `.github/workflows/build-apk.yml`.
4. No repositório, abra **Actions** e selecione **Build VendeAI APK**.
5. Toque em **Run workflow** e confirme.
6. Quando o trabalho terminar com sucesso, abra a execução e baixe o artefato **VendeAI-APK**. Descompacte o arquivo baixado; dentro estará `app-debug.apk`.
7. No Android, abra o APK e autorize a instalação desta fonte se o sistema pedir.

## Limitações importantes
- O APK é uma embalagem Android do protótipo atual. Não adiciona IA real, contas, sincronização em nuvem, pagamentos ou backend.
- Os dados ficam no armazenamento local do aplicativo/aparelho. Desinstalar o app pode apagar os dados.
- O APK de depuração é para testes/instalação direta. Para publicar na Google Play, será necessário gerar uma versão assinada e concluir as exigências atuais da loja.
- O workflow compila o APK na infraestrutura do GitHub; este ZIP por si só não é um APK compilado.
