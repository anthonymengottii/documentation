<div align="center">
  <img src="logo/light.png" alt="UPay Gateway API" width="200" />
  
  # UPay Gateway API - Documentação Pública
  
  [![Documentation](https://img.shields.io/badge/Documentation-Live-brightgreen)](https://docs.upay.com.br)
  [![API Version](https://img.shields.io/badge/API-v1.0-blue)](https://api.upay-sistema.onrender.com)
  [![License](https://img.shields.io/badge/License-MIT-purple)](LICENSE)
  
  **Documentação oficial e completa da API UPay Gateway**
  
  Plataforma completa de pagamentos com PIX, cartão de crédito/débito, boleto bancário e muito mais.
</div>

---

## 📋 Sobre

A **UPay Gateway API** é uma solução completa de processamento de pagamentos desenvolvida para oferecer integração simples, segura e eficiente. Esta documentação fornece todas as informações necessárias para desenvolvedores integrarem pagamentos em suas aplicações.

### Características Principais

- ✅ **API RESTful moderna** - Endpoints intuitivos e bem documentados
- ✅ **Múltiplos métodos de pagamento** - PIX, Cartão de Crédito/Débito e Boleto Bancário
- ✅ **Links de pagamento personalizados** - Crie e compartilhe links únicos com configurações flexíveis
- ✅ **Gestão completa de produtos** - Catálogo integrado com controle de estoque
- ✅ **Sistema de cupons** - Descontos percentuais ou valores fixos com regras configuráveis
- ✅ **Webhooks em tempo real** - Notificações instantâneas sobre eventos importantes
- ✅ **Dashboard administrativo** - Interface completa para gerenciamento e relatórios
- ✅ **Documentação interativa** - Exemplos práticos e referência completa da API

## 🚀 Início Rápido

### Para Desenvolvedores

1. **Obtenha suas credenciais de API**
   - Acesse o [Dashboard UPay](https://upay-sistema.onrender.com)
   - Complete o processo de verificação (KYC)
   - Gere sua API Key em **Configurações → Credenciais de API**

2. **Faça sua primeira requisição**
   ```bash
   curl -X GET "https://api.upay-sistema.onrender.com/api/v1/payment-links" \
     -H "Authorization: Bearer SUA_API_KEY" \
     -H "Content-Type: application/json"
   ```

3. **Explore a documentação**
   - [Guia de Início Rápido](/pages/quickstart)
   - [Referência Completa da API](/api-reference/openapi.json)
   - [Exemplos de Código](/pages/introduction)

### Para Contribuidores da Documentação

Esta documentação é construída com [Mintlify](https://mintlify.com), uma plataforma moderna para documentação técnica.

#### Pré-requisitos

- Node.js 16+ instalado
- npm ou yarn

#### Instalação e Desenvolvimento Local

```bash
# Clone o repositório
git clone https://github.com/anthonymengottii/documentation.git
cd documentation

# Instale o Mintlify CLI globalmente
npm install -g mintlify

# Instale as dependências do projeto
mintlify install

# Inicie o servidor de desenvolvimento
mintlify dev
```

A documentação estará disponível em `http://localhost:3000` com hot-reload ativado.

## 📚 Estrutura do Projeto

```
documentation/
├── api-reference/          # Especificação OpenAPI e referência de endpoints
│   └── openapi.json        # Especificação OpenAPI 3.0.3 completa
├── pages/                  # Conteúdo principal da documentação
│   ├── guides/             # Guias e tutoriais detalhados
│   │   └── features/       # Guias específicos por funcionalidade
│   ├── payment-links/      # Documentação de Links de Pagamento
│   ├── products/           # Documentação de Produtos
│   ├── coupon/             # Documentação de Cupons
│   ├── transactions/       # Documentação de Transações
│   ├── webhooks/           # Documentação de Webhooks
│   └── balance/            # Documentação de Saldo
├── images/                 # Imagens e assets visuais
├── logo/                   # Logos para temas claro e escuro
├── custom.css              # Estilos customizados (scrollbar, etc.)
├── docs.json               # Configuração principal do Mintlify
├── favicon.ico             # Ícone do site
└── README.md               # Este arquivo
```

## 🔧 Desenvolvimento

### Comandos Úteis

```bash
# Iniciar servidor de desenvolvimento
mintlify dev

# Validar configuração
mintlify validate

# Build para produção (local)
mintlify build
```

### Adicionando Novo Conteúdo

1. **Nova página de guia**: Adicione arquivo `.mdx` em `pages/guides/`
2. **Novo endpoint**: Atualize `api-reference/openapi.json` e crie página em `pages/[recurso]/`
3. **Atualizar navegação**: Edite `docs.json` na seção `navigation`

### Convenções

- Use Markdown/MDX para formatação
- Siga a estrutura de pastas existente
- Mantenha consistência com o tom e estilo da documentação
- Inclua exemplos de código quando relevante

## 🚀 Deploy

O deploy é **automático** através da integração do Mintlify com GitHub:

1. Faça push para a branch `main`
2. O Mintlify detecta as alterações automaticamente
3. A documentação é atualizada em alguns minutos

**URL da Documentação**: [https://docs.upay.com.br](https://docs.upay.com.br)

> **Nota**: Certifique-se de que todas as alterações foram testadas localmente antes de fazer push.

## 📖 Recursos da API

### Endpoints Principais

| Recurso | Descrição | Documentação |
|---------|-----------|--------------|
| **Links de Pagamento** | Crie e gerencie links personalizados | [Ver Documentação](/pages/payment-links/reference) |
| **Produtos** | Gerencie seu catálogo de produtos | [Ver Documentação](/pages/products/reference) |
| **Cupons** | Sistema completo de cupons de desconto | [Ver Documentação](/pages/coupon/reference) |
| **Transações** | Consulte e gerencie transações | [Ver Documentação](/pages/transactions/reference) |
| **Webhooks** | Configure notificações em tempo real | [Ver Documentação](/pages/webhooks/reference) |
| **Saldo** | Consulte saldo e movimentações | [Ver Documentação](/pages/balance/reference) |

### Autenticação

A API utiliza autenticação via **API Key** (Bearer Token). Todas as requisições autenticadas devem incluir o header:

```
Authorization: Bearer SUA_API_KEY
```

Para mais detalhes, consulte a [documentação de autenticação](/pages/authentication).

## 🔗 Links Importantes

### Documentação e Recursos

- **Documentação Online**: [https://docs.upay.com.br](https://docs.upay.com.br)
- **API Base URL**: `https://api.upay-sistema.onrender.com`
- **Dashboard**: [https://upay-sistema.onrender.com](https://upay-sistema.onrender.com)
- **Status da API**: [Verificar Status](https://status.upay.com.br)

### Repositórios

- **Documentação**: [GitHub Repository](https://github.com/anthonymengottii/documentation)
- **Sistema Principal**: [GitHub Repository](https://github.com/anthonymengottii/upay_sistema)

### Suporte

- **Email**: [suporte@upay.com.br](mailto:suporte@upay.com.br)
- **Issues**: [GitHub Issues](https://github.com/anthonymengottii/documentation/issues)
- **Documentação de Suporte**: [Páginas de Ajuda](/pages/introduction)

## 🤝 Contribuindo

Contribuições são bem-vindas! Se você encontrar erros, tiver sugestões ou quiser adicionar conteúdo:

1. Abra uma [Issue](https://github.com/anthonymengottii/documentation/issues) descrevendo sua proposta
2. Faça um Fork do repositório
3. Crie uma branch para sua alteração (`git checkout -b feature/minha-contribuicao`)
4. Faça commit das alterações (`git commit -m 'Adiciona nova funcionalidade'`)
5. Faça push para a branch (`git push origin feature/minha-contribuicao`)
6. Abra um Pull Request

## 📝 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

---

<div align="center">
  <p>
    <strong>UPay Gateway API</strong> - Simplificando pagamentos online
  </p>
</div>
