# 🖊️ Assina Fácil

> A solução definitiva, gratuita e sem instalação para assinar documentos digitais com qualidade profissional diretamente do navegador.

![Badge](https://img.shields.io/badge/Status-Stable-green) ![Badge](https://img.shields.io/badge/Plataforma-Mobile%20%26%20Desktop-blue) ![Badge](https://img.shields.io/badge/Privacidade-100%25%20Offline-lightgrey)

## 🎯 O Problema
O fluxo tradicional de "Receber PDF no WhatsApp > Imprimir > Assinar > Escanear > Enviar de volta" é lento, caro e desperdiça papel. Os aplicativos de loja são cheios de anúncios, marcas d'água ou assinaturas mensais.

## 🚀 A Solução
O **Assina Fácil** é um Web App (PWA) de código aberto que permite carregar um documento, selecionar a área exata da assinatura e assinar com o dedo ou mouse com alta precisão.

### ✨ Principais Funcionalidades

* **📂 Compatibilidade Total:** Aceita **PDF**, JPG, PNG, WebP e BMP. Abre arquivos diretamente do Gerenciador de Arquivos, Downloads ou Galeria.
* **✂️ Crop-to-Sign (Recorte Proporcional):** Você desenha um retângulo onde quer a assinatura e o app cria uma área de desenho **proporcional** àquele espaço. Sem distorções ou assinaturas esticadas.
* **📱 Force Landscape (Mobile):** No celular, o app força matematicamente a interface de assinatura para a horizontal, garantindo espaço amplo para assinar, mesmo que o usuário não gire o aparelho.
* **✒️ Caneta "Bic" Realista:** Algoritmo de Curvas de Bézier Quadráticas que simula a pressão e fluidez de uma caneta esferográfica azul real.
* **🖥️ Engine HD 4K:** Detecta a densidade de pixels (DPI) do dispositivo. Funciona com nitidez máxima tanto em celulares modestos quanto em monitores Desktop Quad HD/4K.
* **↩️ Histórico de Edição:** Errou? Desfaça a última assinatura sem perder o documento.
* **🔒 Privacidade Absoluta:** Todo o processamento é feito no navegador do seu dispositivo. **Nenhum dado é enviado para servidores externos.**

---

## 🛠️ Como Usar

1.  **Abrir:** Acesse o link do projeto.
2.  **Carregar:** Clique em **"Abrir Documento"** e escolha a imagem ou PDF (do WhatsApp, Downloads, etc.).
3.  **Ajustar:** Se a foto estiver deitada, use os botões de rotação (↺ ↻) no topo.
4.  **Selecionar:** Arraste o dedo (ou mouse) sobre a linha onde deseja assinar.
5.  **Assinar:**
    * Uma tela cheia branca abrirá.
    * Assine na linha pontilhada.
    * Clique em **Confirmar**.
6.  **Finalizar:** Clique em **"Enviar Whats"** para compartilhar direto ou **"Baixar"** para salvar na galeria.

---

## 🔧 Instalação (Desenvolvedores)

Este projeto é "Zero Dependency" (exceto pela biblioteca PDF.js servida via CDN). Não requer `npm install` ou build complexo.

### Rodando Localmente
1.  Clone o repositório.
2.  Abra o arquivo `index.html` diretamente no navegador ou use uma extensão como **Live Server** no VS Code.

### Deploy (GitHub Pages)
1.  Suba o arquivo `index.html` para um repositório no GitHub.
2.  Vá em **Settings > Pages**.
3.  Em **Source**, selecione `Deploy from a branch` (main).
4.  O link será gerado automaticamente (ex: `seu-usuario.github.io/assina-facil`).

---

## 🧠 Detalhes Técnicos

* **Core:** HTML5, CSS3, Vanilla JavaScript (ES6+).
* **PDF Engine:** `pdf.js` (Mozilla) para renderização de PDFs em Canvas.
* **Matrix Engine V20:** Lógica customizada para mapear coordenadas de toque (`touchmove`) invertidas quando o CSS força a rotação de 90 graus em dispositivos móveis verticais.
* **Canvas API:** Uso de `devicePixelRatio` para super-sampling de imagem, evitando serrilhados em telas de alta resolução.

---

## 📄 Licença

Este projeto é distribuído sob a licença **MIT**. Sinta-se livre para modificar, distribuir e usar profissionalmente.

---
*Desenvolvido com foco em UX e Produtividade.*
