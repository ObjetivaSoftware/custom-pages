# Custom Error Pages - Gestor Imobiliária

Páginas de erro personalizadas para Cloudflare Pages do **Gestor Imobiliária** - Software de gestão imobiliária completo há mais de 10 anos no mercado.

## 📋 Conteúdo

Este repositório contém páginas de erro bonitas e profissionais para todos os principais códigos HTTP:

### Erros do Cliente (4xx)
- **403.html** - Acesso Negado (Forbidden)
- **404.html** - Página Não Encontrada (Not Found)

### Erros do Servidor (5xx)
- **500.html** - Erro Interno do Servidor (Internal Server Error)
- **502.html** - Gateway Indisponível (Bad Gateway)
- **503.html** - Serviço Temporariamente Indisponível (Service Unavailable)
- **504.html** - Tempo de Resposta Excedido (Gateway Timeout)
- **505.html** - Versão HTTP Não Suportada (HTTP Version Not Supported)

### Erros Específicos do Cloudflare (520-524)
- **520.html** - Erro Desconhecido do Servidor (Unknown Error)
- **521.html** - Servidor Recusou Conexão (Web Server Is Down)
- **522.html** - Conexão Expirou (Connection Timed Out)
- **523.html** - Servidor Inalcançável (Origin Is Unreachable)
- **524.html** - Timeout Atingido (A Timeout Occurred)

## ✨ Características

- ✅ **Design Moderno e Profissional** - Interface limpa e agradável
- ✅ **100% Responsivo** - Funciona perfeitamente em mobile, tablet e desktop
- ✅ **Zero Dependências** - Apenas HTML, CSS e JavaScript puro
- ✅ **Animações Suaves** - Transições e efeitos em CSS
- ✅ **Paleta de Cores Única** - Cada erro tem seu gradiente característico
- ✅ **Informações de Contato** - Links diretos para suporte
- ✅ **SEO Otimizado** - Meta tags apropriadas
- ✅ **Acessibilidade** - Seguindo boas práticas de a11y

## 🎨 Identidade Visual

Cada página possui um gradiente único para facilitar identificação:

| Erro | Cores | Descrição |
|------|-------|-----------|
| **403** | `#ff6b6b → #ee5a6f` | Vermelho - Acesso negado |
| **404** | `#6a11cb → #2575fc` | Azul/Roxo - Página não encontrada |
| **500** | `#667eea → #764ba2` | Roxo/Violeta - Erro crítico do servidor |
| **502** | `#f093fb → #f5576c` | Rosa/Vermelho - Problemas de gateway |
| **503** | `#4facfe → #00f2fe` | Azul Claro - Serviço indisponível |
| **504** | `#fa709a → #fee140` | Rosa/Amarelo - Timeout |
| **505** | `#8e2de2 → #4a00e0` | Roxo Escuro - Versão HTTP |
| **520** | `#ff9a56 → #ff6a88` | Laranja/Rosa - Cloudflare erro desconhecido |
| **521** | `#fc5c7d → #6a82fb` | Rosa/Azul - Servidor offline |
| **522** | `#f857a6 → #ff5858` | Rosa/Vermelho - Timeout de conexão |
| **523** | `#ff6b95 → #ffa34d` | Rosa/Laranja - Servidor inalcançável |
| **524** | `#fcb69f → #ff6b6b` | Pêssego/Vermelho - Timeout HTTP |

## 🚀 Como Usar no Cloudflare Pages

### Método 1: Deploy via Git (Recomendado)

1. Faça fork ou clone este repositório
2. Conecte ao Cloudflare Pages:
   - Acesse [Cloudflare Dashboard](https://dash.cloudflare.com/)
   - Vá em **Pages** > **Create a project**
   - Conecte seu repositório Git
   - Configure:
     - **Build command:** (deixe vazio)
     - **Build output directory:** `/`

3. Deploy automático!

### Método 2: Upload Manual

1. Acesse Cloudflare Dashboard
2. Vá em **Pages** > **Create a project** > **Upload assets**
3. Faça upload de todos os arquivos (`.html`, `_redirects`, `_headers`)

### Método 3: Wrangler CLI
```
custom-pages/
├── 403.html              # Acesso negado
├── 404.html              # Página não encontrada
├── 500.html              # Erro interno do servidor
├── 502.html              # Gateway indisponível
├── 503.html              # Serviço indisponível
├── 504.html              # Timeout
├── 505.html              # Versão HTTP não suportada
├── 520.html              # Cloudflare: Erro desconhecido
├── 521.html              # Cloudflare: Servidor recusou conexão
├── 522.html              # Cloudflare: Conexão expirou
├── 523.html              # Cloudflare: Servidor inalcançável
├── 524.html              # Cloudflare: Timeout atingido
├── _redirects            # Configuração de redirecionamentos
├── _headers              # Cabeçalhos HTTP de segurança
├── CLOUDFLARE_SETUP.md   # Guia detalhado de configuração
├── LICENSE               # Licença do projeto
└── README.md             # Este arquivo
``` 502.html              # Gateway indisponível
├── 503.html              # Serviço indisponível
├── 504.html              # Timeout
├── _redirects            # Configuração de redirecionamentos
├── _headers              # Cabeçalhos HTTP de segurança
├── CLOUDFLARE_SETUP.md   # Guia detalhado de configuração
├── LICENSE               # Licença do projeto
└── README.md             # Este arquivo
```

## 🔧 Configuração

Os arquivos `_redirects` e `_headers` já estão configurados para:

- Mapear códigos HTTP para páginas específicas
- Definir cabeçalhos de segurança (CORS, XSS Protection, etc.)
- Desabilitar cache para páginas de erro
- Configurar Content-Type apropriado
Acesse:
- http://localhost:8000/403.html
- http://localhost:8000/404.html
- http://localhost:8000/500.html
- http://localhost:8000/502.html
- http://localhost:8000/503.html
- http://localhost:8000/504.html
- http://localhost:8000/505.html
- http://localhost:8000/520.html
- http://localhost:8000/521.html
- http://localhost:8000/522.html
- http://localhost:8000/523.html
- http://localhost:8000/524.html
```bash
# Python 3
python -m http.server 8000

# Node.js
npx http-server -p 8000

# PHP
php -S localhost:8000
```

Acesse:
- http://localhost:8000/500.html
- http://localhost:8000/502.html
- http://localhost:8000/503.html
- http://localhost:8000/504.html

## 💡 Funcionalidades JavaScript

Cada página inclui recursos opcionais (desativados por padrão):

- **Auto-reload** - Recarrega automaticamente após X segundos
- **Status Check** - Verifica periodicamente se o servidor voltou
- **Retry Counter** - Mostra contagem regressiva para próxima tentativa
- **Error Logging** - Registra erros no console para debug

Para ativar, edite as variáveis no final de cada arquivo HTML.

## 📞 Informações de Contato

As páginas incluem:

- **Email:** suporte@objetivasoftware.com.br
- **WhatsApp:** (54) 98431-1069
- **Site:** https://gestorimobiliaria.com.br
- **Horário:** Segunda a Sexta, 08h30-12h e 13h-17h30

## 🔒 Segurança

Cabeçalhos de segurança configurados no `_headers`:

- `X-Content-Type-Options: nosniff`
- `X-Frame-Options: DENY`
- `X-XSS-Protection: 1; mode=block`
- `Referrer-Policy: strict-origin-when-cross-origin`
- `Permissions-Policy` restritivas

## 📱 Responsividade

Breakpoints otimizados:

- **Desktop:** > 768px (layout padrão)
- **Mobile:** ≤ 768px (layout adaptado, botões em coluna)

## 🎯 Sobre o Gestor Imobiliária

O **Gestor Imobiliária** é um software completo para:

- Corretores e Imobiliárias
- Administradoras de Condomínios
- Gestão de Vendas e Locações
- CRM Integrado
- Site Otimizado para Imóveis

Com mais de **10 anos no mercado**, atendendo empresas em todo o Brasil.

🌐 **Site:** https://gestorimobiliaria.com.br

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 🤝 Suporte

Precisa de ajuda?

- 📧 Email: suporte@objetivasoftware.com.br
- 💬 WhatsApp: (54) 98431-1069
- 🌐 Website: https://gestorimobiliaria.com.br

---

Desenvolvido com ❤️ para o **Gestor Imobiliária** | Objetiva Software © 2026