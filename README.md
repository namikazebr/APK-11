# Lista de Ações — Android App (Capacitor + GitHub Actions)

Aplicativo Android completo com fundo Preto OLED, ilhas flutuantes com luz difusa personalizável (16 cores + Círculo Cromático), submenus por categoria (**Geral**, **Compras**, **Vendas**, **Organização**, **Montagem** + novas abas), cálculo separado de Compras (Pix, à vista, cartão, cupom copiável, loja) e Vendas (lucro/prejuízo em valor e `%`), subtarefas, backup JSON e interface em **Português, Inglês e Espanhol**.

## Como gerar seu `.apk` automaticamente no GitHub (sem instalar nada)

1. Crie um repositório novo no seu GitHub (pode ser **Privado** ou **Público**).
2. Extraia este `.zip` em uma pasta no seu computador e envie todos os arquivos e pastas para a raiz do repositório (incluindo a pasta `.github/workflows/build-apk.yml`).
   - **Pelo navegador:** clique em **uploading an existing file**, selecione todos os arquivos/pastas extraídos (`Ctrl + A`), arraste para a página do GitHub e clique em **Commit changes**.
   - **Via Git no terminal:**
     ```bash
     git init
     git branch -M main
     git add .
     git commit -m "Initial commit Lista de Acoes"
     git remote add origin https://github.com/SEU-USUARIO/SEU-REPO.git
     git push -u origin main
     ```
3. Abra a aba **Actions** no topo do seu repositório no GitHub:
   - O fluxo **Gerar APK Android** vai iniciar sozinho (leva cerca de 2 a 3 minutos).
   - Assim que ficar verde (✅), clique na execução concluída e role até a seção **Artifacts** no final da página.
   - Clique em **`ListaDeAcoes-APK`** para baixar o arquivo contendo o seu `ListaDeAcoes.apk` pronto para instalar no Android!
