# SmythOS UI - O Construtor Visual de Agentes

[![Homepage](https://img.shields.io/badge/_Homepage-SmythOS-green?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJHSURBVHgBfVNNqBJRFL7jT1IYCeUqcRG+AsGVFLhIJIIHLVq93MRsSgpTWgRudaELBRctBDeB2qpdohsVdSOKok+eBC4UAiNSKX9440PtzYydM9yJqV4eOPfOvff8fd85Q8jFosElHo8fJhIJN71TgTJkj+CjWj6sVqu2KIo7VBCuUCg8VNj9E0iLSyQSuQmOx7VaLS4IAjqKsJ/jx3K5PKlUKg88Ho/p74ok58lkkkXDTCbziuO4rz9BMDvP898Ain04HL7fUVksFp+SyeS93+mn02kODKXHer3OYmbQTalUeoLveI8VbTabNQ36o1wuH0nOdrtdiw4iBTsYDALtdjuhwCsR2mw22e12e1YsFo/+gGC1WvW0MilALpd7Tg3UCo4kY4vFooOEV5SEq/r9/gqSD8GXASVQ6mXqJCgCiIjE7/e7Op3OWa/Xe03fNRhZo1arb7darRcMwxCDwXCN/EeAAw53m832FpJ+xyCIj8dKHA7HOygv7XQ6ryogCAoI4nq9FiViGKl7N7xer03uJe47t9t9KxwO97vdrlyiigYSG43GS7PZfJcG3OGi0+lOpVM0GrVB74+RRGB6Kw+Rz+e7HovF7sDVBC+CwSC2GNsogH4mcou0Wq0KymP0ej25BDKfz09SqdSzUCj00Wg03gfjc8xqMplwJ3D+wrLsgewvYySBQOAAhufxaDT6QIcHp0sEB348Hldms1k5m80eUh8NuUAkdqrV6iP8gRAKHbBTl8ulUfC196+UiSPpdPppPp9/sy/jL4yPfDIO4aFTAAAAAElFTkSuQmCC&logoWidth=14)](https://smythos.com)
[![](https://img.shields.io/badge/📄_Code_License-MIT-green)](LICENSE)

A interface visual completa para construir, implantar e gerenciar agentes de IA inteligentes. A UI do SmythOS oferece um espaço de trabalho intuitivo de arrastar e soltar, onde você pode criar workflows sofisticados de agentes sem escrever código, mantendo ainda a flexibilidade de integrações personalizadas quando necessário. <br/><br/> Se você prefere construir agentes com código, ou quer rodar seus agentes visuais na sua própria máquina sem overhead, confira o [SmythOS Runtime, SDK e CLI](https://github.com/SmythOS/sre)! Ótima comunidade, suporte e tutoriais. Comece em minutos!

![SmythOS Visual Agent Studio](https://github.com/SmythOS/sre/blob/main/docs/images/visual-canvas.png.webp?raw=true)

[🚀 Começando](#início-rápido) | [📖 Documentação](#documentação) | [🐳 Setup Docker](DOCKER_COMPOSE.md) | [🤝 Contribuindo](CONTRIBUTING.md)

## Por que o SmythOS Studio

1. **Construção Visual de Agentes**: Criar agentes de IA deve ser tão intuitivo quanto desenhar um fluxograma.
2. **Do No-Code ao Pro-Code**: Comece com a construção visual, estenda com código personalizado quando precisar.
3. **Arquitetura Aberta**: Construa uma vez, implante em qualquer lugar, com controle total sobre sua infraestrutura.

## Princípios de Design

A UI do SmythOS oferece um **ambiente de desenvolvimento completamente visual** para agentes de IA. Assim como os IDEs modernos tornam o desenvolvimento de software acessível, a UI do SmythOS torna o desenvolvimento de agentes de IA intuitivo e poderoso.

### Desenvolvimento Visual em Primeiro Lugar

A UI do SmythOS oferece uma **interface de arrastar e soltar** para construir workflows complexos de agentes. Seja conectando LLMs, integrando APIs, processando dados ou orquestrando workflows de múltiplas etapas, tudo é visual e intuitivo.

Essa abordagem torna o desenvolvimento de agentes de IA **acessível a todos** — de analistas de negócio que entendem os processos a desenvolvedores que precisam escalá-los para produção.

**Benefícios-chave:**

- **Construtor Visual Intuitivo**: Componentes de arrastar e soltar para construir workflows complexos de agentes
- **Testes em Tempo Real**: Teste seus agentes instantaneamente enquanto constrói
- **Deploy em Produção**: Deploy com um clique, do desenvolvimento à produção
- **Arquitetura Extensível**: Adicione componentes e integrações personalizadas
- **Desenvolvimento Colaborativo**: Compartilhe e colabore em projetos de agentes com sua equipe

## Início Rápido

[![Tutorial do SmythOS Studio](https://github.com/user-attachments/assets/54c12bb7-e6d2-4f0c-bc0f-77f812920802)](https://www.youtube.com/watch?v=iEpW5j-h6BM)

### Método 1: Docker Quick Start

Suba e rode instantaneamente com Docker Compose.

```bash
git clone https://github.com/mauroprojetos-privados/smythos-studio.git
cd smythos-studio
cp .env.compose.example .env
docker compose up -d
```

**Acesse sua aplicação:** http://localhost:6060

🐳 **Setup Docker Completo**: Veja nosso [Guia de Docker Compose](DOCKER_COMPOSE.md) para deploy em containers com SSL automático, banco de dados e cache.

**Solução de problemas**: Se você encontrar problemas durante o setup, confira a [seção de Troubleshooting](DOCKER_COMPOSE.md#troubleshooting) no guia do Docker Compose.

---

### Método 2: Setup de Desenvolvimento Local

Perfeito para desenvolvimento, customização e contribuição ao projeto.

```bash
# Clone o repositório
git clone https://github.com/mauroprojetos-privados/smythos-studio.git
cd smythos-studio

# Copie a configuração do ambiente
cp .env.example .env
# Edite o .env com suas credenciais do banco de dados

# Instale as dependências
pnpm install

# Inicie os servidores de desenvolvimento
pnpm dev
```

**Próximos Passos:**

1. Configure seu banco de dados MySQL no `.env`
2. Configure os subdomínios necessários para os embodiments
3. Comece a construir seu primeiro agente!

📖 **Setup Detalhado**: Veja nosso [Guia de Contribuição](CONTRIBUTING.md) para instruções completas de setup de desenvolvimento.

---

## Estrutura do Repositório

Este monorepo contém a plataforma completa da UI do SmythOS:

### 📱 Pacote App - `packages/app`

A aplicação principal, contendo o construtor visual, o frontend React e os serviços de backend.

**Principais Recursos:**

- **Construtor Visual de Agentes**: Interface de arrastar e soltar para criar workflows de agentes
- **Frontend React**: Interface de usuário moderna e responsiva
- **API Backend**: Serviços RESTful para gerenciamento e execução de agentes
- **Testes em Tempo Real**: Teste e depuração instantânea de agentes

### 🔧 Pacote Middleware - `packages/middleware`

Serviços de API centrais e gerenciamento de banco de dados para a plataforma da UI do SmythOS.

**Recursos:**

- **Gerenciamento de Banco de Dados**: ORM baseado em Prisma com suporte a MySQL
- **Camada de API**: Lógica de negócio centralizada e acesso a dados

### ⚡ Pacote Runtime - `packages/runtime`

O servidor de execução que usa o [SRE Core Engine](https://github.com/SmythOS/sre/tree/main) para executar os agentes.

**Recursos:**

- **Execução de Agentes**: Runtime de alta performance para workflows de agentes
- **Ferramentas de Debug**: Monitoramento e depuração em tempo real
- **Arquitetura Escalável**: Lida com múltiplas execuções concorrentes de agentes
- **Suporte a Embodiments**: Implante agentes como chatbots, APIs e integrações

## Documentação

- **[Guia de Contribuição](CONTRIBUTING.md)** - Configure seu ambiente de desenvolvimento e contribua com o projeto
- **[Setup Docker Compose](DOCKER_COMPOSE.md)** - Deploy em containers com SSL automático, banco de dados e cache
- **[Código de Conduta](CODE_OF_CONDUCT.md)** - Diretrizes e padrões da comunidade

## Contribuindo

Agradecemos contribuições da comunidade! Seja corrigindo bugs, adicionando funcionalidades ou melhorando a documentação, sua ajuda torna a UI do SmythOS melhor para todos.

**Formas de Contribuir:**

- 🐛 Reporte bugs e problemas
- 💡 Sugira novas funcionalidades e melhorias
- 🔧 Envie pull requests com correções e melhorias
- 📖 Melhore a documentação e exemplos
- 🎨 Melhore o design de UI/UX

**Comece Agora:**

1. Leia nosso [Guia de Contribuição](CONTRIBUTING.md)
2. Confira as [issues em aberto](https://github.com/mauroprojetos-privados/smythos-studio/issues)

## Colaboradores

<a href="https://github.com/mauroprojetos-privados/smythos-studio/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=mauroprojetos-privados/smythos-studio" />
</a>

## Comunidade & Suporte

- **🐛 Issues**: [Reporte bugs](https://github.com/mauroprojetos-privados/smythos-studio/issues) e solicite funcionalidades
- **📧 Email**: Contate-nos em support@smythos.com para consultas empresariais
- **🌐 Website**: Visite [SmythOS.com](https://smythos.com) para mais informações

## Licença

Este projeto é licenciado sob a [Licença MIT](LICENSE).

**Pronto para construir seu primeiro agente de IA?**

🚀 [Comece Agora](#início-rápido) | 🌟 [Marque este repo com estrela](https://github.com/mauroprojetos-privados/smythos-studio)

---

**/smɪθ oʊ ɛs juː aɪ/**

_Construa visualmente. Implante globalmente. Escale infinitamente._
