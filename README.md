# 🌤️ Clima Extension

Uma **extensão de navegador** que exibe a previsão do tempo para cidades do Brasil, com dados do OpenWeatherMap e listas de estados/municípios do IBGE.

O backend da aplicação está hospedado no **Render** e os arquivos do backend estão na pasta `backend/`.

---

## 🗂 Estrutura do projeto

```
clima-extension/
│
├─ backend/                # Arquivos do backend (Node.js/Express)
│   ├─ index.js
│   └─ package.json
│
├─ popup.html              # Interface da extensão
├─ popup.js                # Lógica do frontend
├─ styles.css              # Estilos da extensão
├─ manifest.json           # Manifesto da extensão
└─ README.md
```

---

## ⚡ Funcionalidades

* 🌎 Seleção de **estado** e **município** com dados do IBGE.
* ⛅ Previsão do tempo detalhada (temperatura, sensação, umidade e chance de chuva) para os próximos dias.
* ⭐ Marque uma cidade como **favorita** e ela será lembrada.
* 💾 **Cache de 10 minutos** para reduzir requisições desnecessárias.
* 🖼️ Cards estilizados com **gradientes e ícones** de clima.
* 🔔 Tooltip com informações detalhadas ao passar o mouse sobre cada horário.

---

## 🚀 Como usar

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/clima-extension.git
```

2. Abra o navegador Chrome/Edge e acesse:

```
chrome://extensions/ (ou edge://extensions/)
```

3. Ative o **Modo de desenvolvedor**.

4. Clique em **Carregar sem compactação** e selecione a pasta `clima-extension/`.

5. Abra a extensão na barra de ferramentas e use a interface para selecionar estado, município e visualizar a previsão.

---

## ☁️ Configurando o Backend no Render

Para que a extensão funcione corretamente, é necessário que o backend esteja ativo:

1. Acesse [Render](https://render.com/) e faça login.
2. Clique em **New Web Service**.
3. Escolha o repositório da pasta `backend/` do projeto.
4. Configure Node.js e a porta padrão (geralmente 10000 ou conforme o `index.js`).
5. Clique em **Deploy**.
6. Após o deploy, copie a URL do serviço e atualize `backendUrl` em `popup.js` com esta URL.

---

## 🛠 Tecnologias

* **Frontend:** HTML, CSS, JavaScript
* **Backend:** Node.js + Express (hospedado no Render)
* **APIs:**

  * OpenWeatherMap (previsão do tempo)
  * IBGE (estados e municípios do Brasil)

---

## 📌 Observações

* A cidade favorita é armazenada no **localStorage**, mantendo sua preferência entre sessões.

---

✨ Aproveite sua previsão do tempo diretamente no navegador!
