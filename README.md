# Recall

Uma ferramenta para análise e processamento de arquivos utilizando o framework Tauri.

## 📥 Downloads

Para usuários que desejam apenas utilizar o programa sem configurar o ambiente de desenvolvimento, baixe a versão mais recente diretamente na página de **Releases**:

👉 [**Baixar Recall (Windows, Mac ou Linux)**](https://github.com/pilati06/recall-tauri/releases)

---

## 🚀 Como executar o projeto (Desenvolvedores)

Para rodar este programa, siga os passos abaixo:

### 1. Pré-requisitos
Certifique-se de ter **Node.js** e **Rust** instalados. Além disso, dependendo do seu sistema operacional:

- **Windows:** Instale as [C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/) (ou o Visual Studio com a carga de trabalho "Desenvolvimento para desktop com C++").
- **macOS:** Execute o comando `xcode-select --install` no terminal para instalar as ferramentas de desenvolvedor.
- **Linux (Ubuntu/Debian):** Execute `sudo apt update && sudo apt install libwebkit2gtk-4.1-dev build-essential curl wget file libxdo-dev libssl-dev libayatana-appindicator3-dev librsvg2-dev`.

### 2. Instalação
No terminal, dentro da pasta do projeto, execute:
```bash
# Instala as dependências do frontend e Tauri
npm install
```

### 3. Execução
Para iniciar o aplicativo em modo de desenvolvimento:
```bash
npm run tauri dev
```

---
*Nota: O primeiro comando `tauri dev` pode demorar um pouco mais pois irá compilar as dependências de Rust.*


### Gerar nova versão no github - tag
No projeto local executar:

Para gerar um patch (1.0.x):
```bash
npm version patch
git push origin main --tags
```
Para gerar uma minor (1.x.-):
```bash
npm version minor
git push origin main --tags
```
Para gerar uma major (x.-.-):
```bash
npm version major
git push origin main --tags
```
