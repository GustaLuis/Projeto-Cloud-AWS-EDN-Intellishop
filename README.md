# Intellishop (E-Commerce com IA)

Este repositório contém a documentação e o planejamento do projeto de conclusão de curso para o programa AWS re/Start, com foco no desenvolvimento de uma plataforma de e-commerce inovadora que utiliza **Inteligência Artificial (IA)** para aprimorar a experiência de compra. A solução aborda a falta de personalização e a dificuldade de descoberta de produtos no varejo digital, visando aumentar a conversão e o engajamento dos clientes.

O projeto foi concebido e documentado pelos alunos **Luis Gustavo Alencar Moura**, **Paula Eduarda Silva** e **Ryan Ricardo de Souza**.

## 📖 Sobre o Projeto
O objetivo geral do projeto é criar uma plataforma de e-commerce de ponta que utilize IA para proporcionar uma experiência de descoberta de produtos superior e personalizada. Para isso, a solução propõe a implementação de um **chatbot** para buscas em linguagem natural e um **sistema de recomendações** personalizadas.

A documentação detalha a arquitetura da solução, baseada nos cinco pilares do **AWS Well-Architected Framework**, garantindo que a plataforma seja robusta, segura, escalável e otimizada em custos.

### 🤖 Funcionalidades Principais (MVP)
O Produto Mínimo Viável (MVP) do projeto inclui as seguintes funcionalidades:
* **Plataforma de E-commerce Essencial:** Funções básicas como cadastro, login, navegação no catálogo, visualização de produtos, carrinho de compras e checkout.
* **Chatbot de Busca (Versão Inicial):** Capacidade de processar consultas em linguagem natural para atributos primários de produtos.
* **Recomendações Simplificadas:** Exibição de produtos relacionados com base em regras simples de associação de itens.

---

## 🛠️ Arquitetura da Solução
A arquitetura foi projetada para ser altamente disponível e resiliente, utilizando uma abordagem **Multi-AZ (Múltiplas Zonas de Disponibilidade)**.

### Serviços AWS Utilizados
* **Amazon CloudFront e AWS WAF:** Atuam como a camada de borda para entrega de conteúdo e segurança, mitigando ataques e garantindo baixa latência.
* **Application Load Balancer (ALB) e Amazon EC2 Auto Scaling:** Gerenciam a distribuição de tráfego e a escalabilidade da camada de aplicação.
* **Amazon RDS Multi-AZ e Amazon ElastiCache:** Camada de dados e cache para garantir alta disponibilidade e performance.
* **Amazon Cognito:** Gerencia a autenticação e identidade dos usuários.
* **Amazon Lex e Amazon OpenSearch Service:** Implementam o chatbot para buscas conversacionais, com OpenSearch indexando e consultando os dados dos produtos.
* **Amazon Personalize:** Utilizado para treinar os modelos e gerar recomendações de produtos personalizadas.

---

## 🚀 Metodologia de Desenvolvimento
O projeto adota uma metodologia ágil, combinando elementos do **Scrum** para o desenvolvimento iterativo e do **Kanban** para a visualização do fluxo de trabalho. O trabalho é dividido em sprints, com ritos como Planejamento de Sprint, Reuniões Diárias e Revisões.

### Sprints Planejadas
* **Sprint 1 - Base Confiável:** Foco na construção da infraestrutura fundamental na AWS usando **"Infrastructure as Code" (IaC)**, incluindo a configuração de rede (VPC Multi-AZ), segurança (CloudFront, WAF) e camadas de dados (RDS, ElastiCache).
* **Sprint 2 – IA Essencial:** Implementação das funcionalidades de IA e autenticação, como a integração com Amazon Cognito, Lex, OpenSearch e Personalize.

---

## 📊 Métricas de Sucesso
O sucesso do projeto será avaliado através de KPIs:
* **Métricas de Negócio:** Taxa de conversão, aumento do ticket médio e retenção de clientes.
* **Métricas de Produto:** Taxa de cliques nas recomendações, taxa de engajamento do chatbot e adoção das funcionalidades de IA.
* **Métricas Técnicas:** Disponibilidade (SLA), latência e saúde da aplicação.

---

## 📄 Licença
Este projeto está sob a licença **MIT**.
