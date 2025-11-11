# 🌱 Marmita Fit da Camilla

Este repositório contém o código do **site de redirecionamento inteligente para o WhatsApp** da marca *Marmita Fit da Camilla*.  
O objetivo é permitir que, ao postar o link em grupos de WhatsApp, o preview mostre **imagem, título e descrição atrativos**, e que ao clicar o usuário seja levado diretamente para uma conversa de pedido com a Camilla.

---

## 💡 Como funciona

O projeto é hospedado gratuitamente via **GitHub Pages**, utilizando apenas um arquivo `index.html` e uma imagem otimizada (`marmita_fit.jpg`).  

O HTML contém:
- **Tags Open Graph (`og:`)** → controlam o preview mostrado no WhatsApp (título, descrição e imagem).
- **Redirecionamento automático** → após 2 segundos, o visitante é levado para o WhatsApp.
- **Botão manual** → usado como alternativa quando o link é aberto dentro do app WhatsApp, que bloqueia redirecionamentos automáticos.
- **Fallback `<noscript>`** → garante o redirecionamento mesmo se o navegador tiver JavaScript desativado.

---

## 🧭 Comportamento inteligente

| Ambiente | O que acontece |
|-----------|----------------|
| **WhatsApp (app mobile)** | Mostra o site e permite clicar no botão para abrir o chat. |
| **Navegador comum (PC ou celular)** | Redireciona automaticamente após 2 segundos. |
| **WhatsApp Web / Desktop** | Redireciona normalmente para o WhatsApp Web. |
| **JavaScript desativado** | Usa fallback automático (`<noscript>`). |



