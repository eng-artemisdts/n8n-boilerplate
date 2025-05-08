# Artemis n8n Boilerplate

Este repositório foi criado pela **Artemis** com o objetivo de fornecer uma base inicial para projetos de automação utilizando o [n8n](https://n8n.io/), uma poderosa ferramenta de automação de workflows de código aberto.

## 👉 Sobre o Projeto

Este boilerplate contém uma configuração mínima e funcional do n8n utilizando Docker Compose. Ele permite iniciar rapidamente projetos que utilizam automações, integrações e workflows personalizados.

Além disso, acompanha uma pasta `workflows/` contendo as exportações de todos os workflows já criados pela equipe da **Artemis**, servindo como referência e ponto de partida para novos projetos.

## 🚀 Como usar

### Pré-requisitos

* [Docker](https://www.docker.com/)
* [Docker Compose](https://docs.docker.com/compose/)

### Iniciando o ambiente

1. Clone este repositório:

   ```bash
   git clone https://github.com/artemis-tech/n8n-boilerplate.git
   cd n8n-boilerplate
   ```

2. Suba os containers:

   ```bash
   docker-compose up -d
   ```

3. Acesse o n8n em:

   ```
   http://localhost:5678
   ```

> A primeira vez pode demorar um pouco, pois o Docker irá baixar as imagens necessárias.

## 📂 Estrutura

```
n8n-boilerplate/
├── docker-compose.yml   # Configuração do serviço n8n
├── workflows/            # Workflows exportados pela Artemis
└── README.md             # Documentação do projeto
```

## ⚙️ Configuração

As variáveis de ambiente estão definidas diretamente no `docker-compose.yml`, mas podem ser extraídas para um `.env` caso deseje customizações mais avançadas.

## 🛡️ Segurança

Este boilerplate não possui autenticação habilitada por padrão. Para uso em produção, **recomenda-se configurar variáveis como**:

* `N8N_BASIC_AUTH_USER`
* `N8N_BASIC_AUTH_PASSWORD`
* `N8N_ENCRYPTION_KEY`

Consulte a [documentação oficial](https://docs.n8n.io/hosting/docker/) para mais detalhes.

## 📘 Documentação oficial

* [n8n Docs](https://docs.n8n.io/)
* [n8n GitHub](https://github.com/n8n-io/n8n)

---

Feito com 💙 pela equipe da **Artemis**.
