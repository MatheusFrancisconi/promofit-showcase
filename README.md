# 🏋️‍♂️ PromoFIT - Showcase

> **Aviso:** Este é um repositório de demonstração. O código-fonte do PromoFIT é mantido de forma privada para proteger as credenciais de integração, a lógica do agendamento inteligente e as regras de filtragem de afiliados.

## 📌 Sobre o Projeto

O **PromoFIT** é um grupo de ofertas especializadas em suplementos e fitness. O sistema backend consiste em um bot de afiliados totalmente automatizado que garimpa as melhores ofertas em marketplaces como Shopee e Mercado Livre. 

O foco da aplicação não é apenas extrair links, mas aplicar inteligência ao processo: o bot filtra os achados com critérios de qualidade rigorosos, gera mensagens persuasivas com copywriting variado e realiza a transmissão dessas ofertas para grupos do WhatsApp utilizando um sistema de agendamento inteligente.

## 🛠️ Tecnologias e Arquitetura

A automação foi estruturada para garantir conversão de vendas e estabilidade no envio de mensagens:

*   **Garimpo de Dados:** [Insira a linguagem/ferramenta, ex: Node.js, Puppeteer, APIs de Afiliados]
*   **Integração WhatsApp:** [Ex: Baileys, WhatsApp Web.js ou API Oficial]
*   **Hospedagem e Execução:** [Ex: AWS, VPS Linux, Heroku]

## ✨ Principais Funcionalidades

*   **Scraping e Garimpo Ativo:** Rastreio constante de produtos de alta demanda no nicho fitness diretamente na Shopee e no Mercado Livre.
*   **Filtros de Qualidade:** Algoritmo que avalia reputação do vendedor, percentual real de desconto e avaliações do produto antes de aprovar a oferta.
*   **Motor de Copywriting Variado:** Geração dinâmica de textos persuasivos (gatilhos de urgência, escassez e benefícios) para acompanhar os links de afiliados, evitando que as mensagens do grupo se tornem repetitivas.
*   **Agendamento Inteligente:** Sistema de filas e delays para o disparo no WhatsApp, garantindo que as mensagens sejam enviadas nos horários de maior pico de conversão e evitando penalizações na plataforma.

## 💻 Desafios Técnicos e Aprendizados

Durante o desenvolvimento deste sistema comercial, os principais desafios de engenharia resolvidos foram:
*   **Normalização de Dados:** Padronizar as informações (título, preço, imagem) vindas de estruturas JSON e HTML completamente diferentes (Shopee vs. Mercado Livre).
*   **Prevenção de Banimento (Anti-Spam):** Criação da lógica de "agendamento inteligente" para cadenciar o envio de mensagens, simulando o comportamento humano.
*   **Manutenção de Sessão:** Gerenciamento da conexão com o WhatsApp de forma persistente em um ambiente de servidor, lidando com quedas de conexão e reconexões automáticas.

## 📸 Demonstração Visual

Abaixo está um exemplo prático do funcionamento da aplicação, desde a geração do copy até o envio no grupo:

![Exemplo de Mensagem PromoFIT no WhatsApp](link-da-imagem-do-whatsapp-aqui.jpg)
*Legenda: Oferta de suplemento processada, formatada com copy dinâmico e enviada automaticamente pelo PromoFIT no WhatsApp.*

---
*Desenvolvido e mantido por [Matheus Francisconi](https://github.com/MatheusFrancisconi).*
