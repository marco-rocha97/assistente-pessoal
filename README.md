# Assistente de Conteúdo Inteligente 🤖

> Uma automação que transforma suas ideias soltas em conteúdo estruturado e organizado automaticamente no ClickUp

![Badge](https://img.shields.io/badge/n8n-Automation-FF6D5A?style=flat-square&logo=n8n)
![Badge](https://img.shields.io/badge/Telegram-Bot-26A5E4?style=flat-square&logo=telegram)
![Badge](https://img.shields.io/badge/OpenAI-GPT4-412991?style=flat-square&logo=openai)
![Badge](https://img.shields.io/badge/ClickUp-Tasks-7B68EE?style=flat-square&logo=clickup)
![Badge](https://img.shields.io/badge/Redis-Buffer-DC382D?style=flat-square&logo=redis)
![Badge](https://img.shields.io/badge/Status-Active-success?style=flat-square)

## 🎯 O que essa automação faz?

Sabe quando você tem uma ideia genial no meio do dia e precisa anotar em algum lugar? 
Esta automação pega essas suas ideias "bagunçadas" e transforma em conteúdo profissional e estruturado automaticamente!

Você pode enviar **qualquer tipo de conteúdo** - texto, áudio, imagem ou documento - e a IA organiza tudo em tópicos claros, adaptados para diferentes redes sociais, criando uma tarefa completa no seu ClickUp.

## ⚡ Como funciona na prática?

1. **📱 Você envia uma mensagem** no Telegram (texto, áudio, foto ou PDF)
2. **🧠 A IA processa** o conteúdo usando diferentes tecnologias:
   - Áudios são transcritos automaticamente
   - Imagens são analisadas e descritas
   - PDFs têm o texto extraído
   - Textos são organizados diretamente
3. **⏱️ Sistema inteligente de buffer** aguarda 15 segundos para você enviar mensagens complementares
4. **🎨 IA especialista em conteúdo** organiza suas ideias em estrutura profissional
5. **✅ Tarefa criada no ClickUp** com título e conteúdo estruturado em tópicos
6. **📲 Confirmação no Telegram** de que o conteúdo foi processado

## 💼 Casos de uso reais

### 🎯 Caso principal - Consultores e PMEs
**Cenário:** Você está no trânsito e tem uma ideia para um post no LinkedIn sobre automação
- Envia áudio: "Cara, hoje vi uma empresa perdendo 3 horas por dia só organizando planilhas..."
- **Resultado:** Tarefa no ClickUp com post estruturado, ganchos profissionais e CTAs

### 🎓 Educação e Cursos
**Cenário:** Professor tem insights sobre metodologia de ensino
- Envia foto de anotações da aula
- **Resultado:** Post estruturado para LinkedIn Educacional com storytelling pedagógico

### 🏠 Arquitetura e Design
**Cenário:** Arquiteto visita obra e tem insights sobre tendências
- Envia foto do ambiente + áudio explicativo
- **Resultado:** Conteúdo para Pinterest/Instagram com análise técnica acessível

## 📋 O que você precisa ter

### 🔧 Ferramentas necessárias
- **n8n** instalado e configurado
- **Conta no Telegram** com bot criado
- **API OpenAI** (para transcrição e análise)
- **Conta ClickUp** com workspace configurado
- **Redis** para sistema de buffer (pode usar Redis Cloud gratuito)

### 🔑 Credenciais necessárias
- Token do Bot Telegram
- API Key OpenAI
- Credenciais OAuth2 ClickUp
- Configuração Redis (host, porta, senha se necessário)

## 🚀 Como colocar para funcionar

### Passo 1: Configurar o Bot do Telegram
1. Converse com [@BotFather](https://t.me/botfather) no Telegram
2. Crie um novo bot com `/newbot`
3. Guarde o token fornecido
4. Configure o webhook no n8n

### Passo 2: Configurar APIs no n8n
1. **OpenAI:** Adicione sua API key nas credenciais
2. **ClickUp:** Configure OAuth2 e autorize o acesso
3. **Redis:** Configure conexão (local ou cloud)
4. **Telegram:** Adicione o token do bot

### Passo 3: Ajustar configurações do ClickUp
1. Identifique o ID do seu Team
2. Encontre o ID do Space desejado
3. Configure o ID da Lista onde as tarefas serão criadas
4. Atualize os parâmetros no nó "Create Task"

### Passo 4: Personalizar o prompt da IA
1. Abra o nó "Content Agent"
2. Ajuste o prompt para seu nicho/público
3. Modifique exemplos e linguagem conforme necessário

### Passo 5: Testar o workflow
1. Ative o workflow no n8n
2. Envie uma mensagem teste para seu bot
3. Verifique se a tarefa foi criada no ClickUp
4. Ajuste configurações se necessário

## 🤝 Quer contribuir ou adaptar?

Este workflow é totalmente customizável! Algumas ideias para melhorar:

- 🔄 Adicionar mais integrações (Notion, Trello, Asana)
- 🎯 Criar templates específicos por nicho
- 📱 Expandir para WhatsApp ou Discord
- 🤖 Adicionar mais modelos de IA

**Dicas para personalização:**
1. Fork este workflow como base
2. Ajuste o prompt para seu público
3. Modifique integrações conforme necessário
4. Teste com pequenos volumes primeiro
5. Documente suas adaptações

## 🆘 Precisa de ajuda?

### 🔧 Problemas comuns
**Bot não responde:**
- Verifique se o webhook está ativo
- Confirme token do Telegram
- Valide configuração do trigger

**IA não processa bem:**
- Ajuste o prompt para seu contexto
- Verifique créditos da OpenAI
- Teste com mensagens mais claras

**ClickUp não cria tarefas:**
- Confirme IDs do workspace/lista
- Verifique permissões OAuth2
- Valide estrutura dos dados

---

**⭐ Se este workflow te ajudou, considere dar uma estrela no repositório!**
