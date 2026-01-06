# We Health

## Sobre o Mermaid

**Mermaid** é uma plataforma JavaScript baseada em Markdown que permite criar diagramas e visualizações de forma fácil e intuitiva, diretamente pelo código. É especialmente útil para documentação técnica, já que permite descrever arquiteturas, fluxos de dados, sequências e muito mais usando uma sintaxe simples.

### Características do Mermaid:
- 📊 Criação de diagramas sem ferramentas gráficas
- 🔄 Suporte a múltiplos tipos de diagramas (fluxogramas, sequências, gráficos, etc.)
- 🌐 Visualização direta no GitHub, GitLab, Notion e outras plataformas
- 💡 Fácil controle de versão através de código
- ⚡ Renderização rápida e responsiva

### Site Oficial:
[https://mermaid.js.org](https://mermaid.js.org)

---

## Diagrama C4 da Arquitetura WeHealth

A arquitetura do WeHealth foi modelada usando a **notação C4** (Context, Containers, Components, Code), que oferece uma visão em diferentes níveis de abstração do sistema.

### O que é C4?
C4 é um método de modelagem de arquitetura que descreve um software através de 4 perspectivas:
1. **C1 - System Context**: Visão geral do sistema e seus atores externos
2. **C2 - Containers**: Componentes principais da aplicação (API, Database, Apps)
3. **C3 - Components**: Componentes internos de um container específico
4. **C4 - Code**: Detalhes de implementação (classes, funções, etc.)

### Como Usar o Código C4 no Mermaid

O código C4 do WeHealth está no arquivo `codigoC4.txt`. Para visualizar os diagramas, você tem duas opções:

#### **Opção 1: Usar o Editor Online do Mermaid**

1. Acesse: [https://mermaid.live](https://mermaid.live)
2. Cole o código do arquivo `codigoC4.txt` na aba de edição
3. Os diagramas serão renderizados automaticamente no lado direito

#### **Opção 2: Visualizar no GitHub**

1. Abra o arquivo `codigoC4.txt` neste repositório
2. O GitHub renderizará automaticamente os diagramas Mermaid

#### **Opção 3: Integrar em Documentação**

Para incluir os diagramas em um arquivo Markdown (como este README), use a sintaxe:

```markdown
```mermaid
[cole o código C4 aqui]
```
```

### Estrutura do Código C4

O arquivo `codigoC4.txt` contém:

- **Pessoas/Atores**: 
  - `UsuarioFinal`: Busca serviços, agenda, avalia, recebe cashback e notificações
  - `Parceiro`: Gerencia página, promoções e assinaturas
  - `Administrador`: Gerencia usuários, parceiros, denúncias e relatórios

- **Sistemas Externos**:
  - Google Maps API
  - MercadoPago
  - Firebase Messaging
  - Cloud Storage

- **Containers do WeHealth**:
  - Mobile App (React Native / Flutter)
  - Admin Web App (Next.js)
  - Backend API (Node.js / TypeScript)
  - Database (PostgreSQL)
  - Auth Service (Supabase Auth / Auth0)
  - Background Worker (Node.js / Bull)
  - Media Service

- **Componentes da API**:
  - AuthController
  - UserController
  - PartnerController
  - BookingController
  - CashbackService
  - NotificationService
  - PaymentService
  - MediaService
  - ReportService

### Visualizações Disponíveis

O código C4 inclui as seguintes visualizações:

1. **C1 - System Context**: Visão geral de todos os atores e sistemas
2. **C2 - Container View**: Componentes principais e integrações
3. **C3 - Component View**: Detalhes dos componentes da Backend API
4. **C4 - Fluxo (Pessoa → Containers)**: Sequência de autenticação e pagamento
5. **C4 - Fluxo Interno (Components)**: Sequência entre componentes da API