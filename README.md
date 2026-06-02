# 🏋️‍♂️ PromoFIT - Showcase

> **Aviso:** Este é um repositório de demonstração. O código-fonte do PromoFIT é mantido de forma privada para proteger as credenciais de integração, a lógica do agendamento inteligente e as regras de filtragem de afiliados.

## 📌 Sobre o Projeto

O **PromoFIT** é um grupo de ofertas especializadas em suplementos e fitness. O sistema backend consiste em um bot de afiliados totalmente automatizado que garimpa as melhores ofertas em marketplaces como Shopee e Mercado Livre. 

O foco da aplicação não é apenas extrair links, mas aplicar inteligência ao processo: o bot filtra os achados com critérios de qualidade rigorosos, gera mensagens persuasivas com copywriting variado e realiza a transmissão dessas ofertas para grupos do WhatsApp utilizando um sistema de agendamento inteligente.

## 🛠️ Tecnologias e Arquitetura

A automação foi estruturada para garantir conversão de vendas, estabilidade no envio de mensagens e alta performance na coleta de dados:

* **Linguagem Principal:** Python
* **Garimpo de Dados:** Integração com a API da Shopee via **GraphQL** e rotinas de **Web Scraping** customizadas para o Mercado Livre.
* **Integração WhatsApp:** EvolutionAPI.
* **Infraestrutura e Hospedagem:** Servidor VPS na Hostinger, garantindo uptime de 24/7 para os agendamentos.

## ✨ Principais Funcionalidades

* **Scraping e Garimpo Ativo:** Rastreio constante de produtos de alta demanda no nicho fitness (suplementos, equipamentos) utilizando APIs diretas e raspagem de dados.
* **Filtros de Qualidade:** Algoritmo que avalia reputação do vendedor, percentual real de desconto e avaliações do produto antes de aprovar a oferta para o grupo.
* **Motor de Copywriting Variado:** Geração dinâmica de textos persuasivos (gatilhos de urgência, escassez e benefícios) para acompanhar os links de afiliados, evitando que as mensagens se tornem repetitivas.
* **Agendamento Inteligente:** Sistema de filas e delays para o disparo no WhatsApp, garantindo que as mensagens sejam enviadas nos horários de maior pico de conversão.

## 💻 Desafios Técnicos e Aprendizados

Durante o desenvolvimento deste sistema comercial, os principais desafios de engenharia resolvidos foram:
* **Normalização de Dados Heterogêneos:** Padronizar as informações (título, preço, imagem) vindas de fontes completamente diferentes, unificando as respostas limpas em JSON do GraphQL da Shopee com a extração bruta de HTML do Mercado Livre.
* **Prevenção de Banimento (Anti-Spam):** Criação da lógica de agendamento inteligente em Python para cadenciar o envio de mensagens via EvolutionAPI, simulando o comportamento humano e respeitando os limites do WhatsApp.
* **Gerenciamento de Infraestrutura:** Configuração e manutenção do ambiente na VPS (Hostinger) para garantir que os scripts de automação rodem continuamente de forma autônoma.

## 📸 Demonstração Visual

Abaixo está um exemplo prático do funcionamento da aplicação, desde a geração do texto persuasivo até o envio final no grupo:

![Exemplo de Mensagem PromoFIT no WhatsApp](link-da-imagem-do-whatsapp-aqui.jpg)
*Legenda: Oferta de suplemento processada, formatada com copy dinâmico e enviada automaticamente pelo PromoFIT no WhatsApp.*

---
*Desenvolvido e mantido por [Matheus Francisconi](https://github.com/MatheusFrancisconi).*
