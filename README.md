# 🚀 Agente Supremo (Termux + PWA + Node)

Agente Supremo é um agente de automação de código full stack, desenvolvido 100% via mobile (Android + Termux), capaz de executar, corrigir e reiniciar projetos de forma controlada através de um painel PWA.

> 🎯 **Diferencial:** projetado e operado diretamente no celular, demonstrando engenharia full stack em ambiente mobile.

---

## ✨ Principais funcionalidades

- 🧠 Painel PWA para controle do agente
- 🔍 Endpoint `/health` para monitoramento
- ⚙️ Endpoint `/run` para execução controlada
- 🛡️ Whitelist de comandos (segurança)
- 🔄 Script `start-all.sh` para subir todo o ambiente
- 🧹 Botão **Auto-corrigir** (clean + reinstall)
- 🟢 Indicador visual de status do backend

---

## 🏗️ Arquitetura

ai-agent/ ├── backend/        # API Node.js do agente ├── pwa/            # Interface PWA (Vite) ├── workspace/      # Área de testes do agente └── scripts/        # Scripts de automação

---

## 🧪 Tecnologias utilizadas

**Frontend**
- Vite
- JavaScript
- PWA

**Backend**
- Node.js
- HTTP nativo
- Exec controlado

**Ambiente**
- Termux (Android)
- Linux shell

---

## ▶️ Como rodar localmente (Termux)

### 1️⃣ Backend

```bash
cd ~/ai-agent/backend
node server.cjs


cd ~/ai-agent/pwa
npm install
npm run dev -- --host



cd ~/ai-agent/pwa
npm install
npm run dev -- --host



🔐 Segurança
O agente utiliza:
whitelist de comandos permitidos
autenticação via header x-agent-token
execução controlada via child_process
isolamento em workspace
🚧 Melhorias de segurança em andamento (hardening progressivo).


🗺️ Roadmap
[ ] Migração para TypeScript
[ ] Testes automatizados
[ ] Deploy online
[ ] UI premium
[ ] Modo IA autônoma



👨‍💻 Autor
Renan Borges
Projeto desenvolvido como evolução prática para posição de Desenvolvedor Full Stack Júnior.


📌 Status do projeto
🟢 Em desenvolvimento ativo
🟢 Funcional localmente
🟡 Em processo de profissionalização

## Testes (Jest)

Execute os testes automatizados do
 backend:

```bash
cd ~/ai-agent/backend
npm test

⭐ Se este projeto te interessou, considere dar uma estrela!
