---
title: Garantia de Produtos
---

# 🛡️ Garantia de Produtos

> 💬 *Sabe aquela geladeira que deu defeito uma semana depois de a garantia acabar? Nunca mais!* 😩➡️😌

[⬅️ Voltar ao início](../index.md) · [📘 Método](../metodo.md)

| 📌 Status | 🧰 Ferramentas | ⚡ Gatilho | 📅 Criada em |
|:---:|---|---|---|
| ✅ Planejada | 📊 Sheets · 📧 Gmail · 📅 Calendar | ☀️ Todo dia às 8h | 23/10/2026 |

---

## 😩 O problema

Garantias vencem em silêncio. Quando o produto quebra, a nota fiscal está perdida e o prazo já passou.

## 🎯 O que a automação faz

- 📬 Manda um e-mail **30 dias** e **7 dias** antes de a garantia vencer
- 📅 Cria um lembrete no Google Calendar na data final
- ✅ Marca na planilha o que já foi avisado, para nunca repetir
- ⌛ Identifica garantias vencidas sem mandar e-mail

## ⚙️ Workflow

```
⏰ Agenda (8h) ➜ 📊 Lê a planilha ➜ 🧮 Calcula ➜ 🔀 Decide o aviso
                                                   ├─ 📬 30 dias ➜ 📅 Calendar ➜ ✅ Marca
                                                   ├─ ⚠️ 7 dias  ➜ ✅ Marca
                                                   └─ ⌛ Vencida ➜ 🏷️ Marca status
```

## 📦 Arquivos completos

Os três passos, o prompt final, o JSON do workflow e o guia de importação estão no repositório da automação:
👉 [github.com/robsonlsgai/garantia-de-produtos](https://github.com/robsonlsgai/garantia-de-produtos)

## 💭 O que aprendi

- ✨ Quanto mais claro o objetivo, o contexto e as regras, mais certeira é a resposta da IA.
- 🧠 Pensar nas exceções antes (e-mail inválido, aviso repetido, garantia vencida) evita dor de cabeça depois.

## 🔮 Próximas melhorias

- [ ] ⚙️ Importar e ativar no N8N
- [ ] 🧾 Ler a nota fiscal recebida por e-mail e cadastrar o produto sozinho
- [ ] 📱 Mandar o aviso também por WhatsApp ou Telegram
