---
title: Método
---

# 📘 Script Mestre: do problema ao workflow N8N

> 🧭 O roteiro que eu sigo para **toda** automação nova. Ele nasceu no Desafio Criativo da DIO e virou o meu método. 💚

[⬅️ Voltar ao início](index.md) · [📝 Modelo em branco](modelo-nova-automacao.md)

---

## 0️⃣ Ideia: o que vale automatizar? 💭

Uma boa candidata tem três características: é **repetitiva** 🔁, tem **regra clara** 📏 e **incomoda** 😩.

Perguntas para achar a próxima:
- 🔁 O que eu faço toda semana, sempre do mesmo jeito?
- 😩 Que esquecimento já me custou dinheiro, tempo ou paz?
- 📬 Onde a informação **chega** (e-mail, formulário, planilha, mensagem) e para onde ela **precisa ir**?
- ⏱️ Quanto tempo por mês eu ganharia se isso rodasse sozinho?

💡 **Banco de ideias:** garantias ⏰ · boletos e contas 💸 · aniversários 🎂 · backup de arquivos 🗄️ · resumo diário de e-mails 📧 · relatório semanal 📊 · lembrete de remédios 💊 · organização de notas fiscais 🧾

---

## 1️⃣ Objetivo: o quê, para quem e para quê 🎯

✍️ Responda:
- 🎯 Qual tarefa eu quero automatizar?
- 👥 Quem usa ou é impactado (eu, minha família, meus clientes)?
- 🏁 Qual resultado deve acontecer, de forma que dê para **ver**?

```text
Quero criar uma automação no N8N para [processo].
Público ou responsável:
[quem utilizará]
Resultado esperado:
[resultado desejado]
```

✅ **Confere?** O processo cabe em **uma frase**? O resultado é concreto (e-mail enviado, linha salva, alerta criado)?

---

## 2️⃣ Contexto e regras: o mapa do fluxo 🔧

✍️ Responda:
- 🧰 Quais ferramentas participam?
- ⚡ O que **dispara** a automação: um horário, um e-mail novo, um formulário?
- 🔄 Quais etapas acontecem, e em que ordem?
- 🚦 Quais regras, validações e exceções existem?

```text
Ferramentas envolvidas:
[lista de ferramentas]
Gatilho:
[o que dispara e quando]
Dados disponíveis:
[colunas da planilha, campos do formulário ou do e-mail]
Fluxo desejado:
1. [etapa 1]
2. [etapa 2]
3. [etapa 3]
4. [registro final: onde fica salvo o que aconteceu]
Regras importantes:
[restrições, validações ou exceções]
```

🧠 **Regras que quase todo mundo esquece:**
- 🚫 E se um campo vier **vazio** ou **inválido**?
- 🔁 Como evitar fazer a **mesma coisa duas vezes**?
- ⌛ E se a data **já passou**?
- 🆘 Quem fica sabendo se **algo der errado**?

💡 **Dica de ouro:** cite os **nomes exatos** das colunas e dos campos. A IA acerta muito mais os nós do N8N quando sabe com quais dados vai trabalhar.

---

## 3️⃣ Prompt final: juntando as peças 🚀

```text
Atue como um especialista em N8N.
Crie uma automação para [processo].
Público:
[público]
Ferramentas envolvidas:
[ferramentas]
Gatilho:
[o que dispara e quando]
Dados disponíveis:
[colunas ou campos]
Fluxo:
[etapas numeradas]
Regras:
[regras]
Explique quais nós do N8N devem ser utilizados e a lógica de funcionamento do workflow.
Ao final, gere o JSON do workflow para importação no N8N, usando espaços reservados no lugar de IDs e credenciais.
```

🔍 **Revisão antes de usar:**
- [ ] 🎯 O objetivo está claro?
- [ ] 🔢 As etapas estão em ordem?
- [ ] 🚦 As regras e exceções foram informadas?
- [ ] 📋 Os dados (colunas e campos) estão nomeados?

🧪 **Teste rápido:** cole o prompt em uma IA. Se ela fizer perguntas antes de responder, ainda falta contexto. Volte ao passo 2️⃣.

---

## 4️⃣ Construção: do JSON ao workflow rodando ⚙️

1. 📥 **Importe** o JSON no N8N (três pontinhos ➜ *Import from File*).
2. 🔑 **Conecte as credenciais** (Google, e-mail, etc.) em cada nó.
3. ✏️ **Troque os espaços reservados** (`COLE_AQUI_O_ID`) pelos valores reais.
4. 🧪 **Teste com dados de mentira** primeiro: uma linha de teste, um e-mail para você mesmo.
5. 🐞 Deu erro? Copie a mensagem do nó e peça ajuda à IA com o contexto do prompt.
6. 🟢 **Ative** o workflow e acompanhe as primeiras execuções.

---

## 5️⃣ Registro: documentar para lembrar 📚

1. 📝 Copie o [modelo de nova automação](modelo-nova-automacao.md) para `automacoes/<nome-da-automacao>.md`.
2. ✍️ Preencha a ficha com os passos 1 a 3 e o que aprendeu.
3. 💾 Guarde o JSON do workflow junto (sem dados sensíveis!).
4. 🗂️ Adicione uma linha no **catálogo** da [página inicial](index.md).
5. 🔄 Atualize o **status** conforme a automação evolui.

🔒 **Segurança sempre:** nunca publique senhas, chaves de API, IDs reais de planilhas ou dados pessoais. Este site é **público**.

---

## 🏁 Checklist de uma automação completa

- [ ] 💭 Ideia escolhida e anotada
- [ ] 🎯 Objetivo definido
- [ ] 🔧 Contexto, dados e regras mapeados
- [ ] 🚀 Prompt final revisado
- [ ] ⚙️ Workflow importado, testado e ativo
- [ ] 📚 Ficha publicada e catálogo atualizado
- [ ] 🔒 Nada sensível publicado

<p align="center">Bora automatizar! 🚀💚</p>
