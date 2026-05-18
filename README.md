# 🤖 Chatbot Ético e Modular com Groq API

Este repositório contém um assistente virtual interativo baseado em terminal que utiliza a API da Groq para interagir com o modelo de linguagem Llama 3. O projeto foi estruturado em Python focado em simplicidade, contendo um sistema de instruções iniciais (*System Prompt*) e gerenciamento de histórico para manter o contexto da conversa.

---

## 🚀 Conceitos do Projeto

* **System Prompt:** Define as regras de comportamento do bot (tom paciente, foco em iniciantes e recusa de pedidos perigosos).
* **Memória de Contexto:** Armazena o histórico da conversa em uma lista para que o modelo lembre do que foi dito anteriormente.
* **Loop de Interação:** Mantém o chat ativo no terminal até que o usuário digite um comando de saída.

---

## 🛠️ Pré-requisitos

Antes de começar, você precisará ter instalado em sua máquina:
* **Python 3.8** ou superior.
* Uma conta e uma chave de API gerada na plataforma da [Groq](https://console.groq.com/).

---

## 🏁 Como Usar: Passo a Passo

Siga as etapas abaixo para configurar e executar o chatbot no seu computador.

### Passo 1: Baixar o código
Crie uma pasta no seu computador e salve o código do chatbot em um arquivo com o nome `chatbot.py`.

### Passo 2: Instalar a biblioteca da Groq
Abra o terminal ou prompt de comando na pasta onde o arquivo foi salvo e instale a dependência necessária executando o seguinte comando:

```bash
pip install groq
```

## Passo 3: Configurar a sua Chave de API
O código está configurado para ler a sua chave de duas maneiras. Escolha uma delas:

* **Opção A (Variável de Ambiente):** Alimente a chave direto no terminal antes de rodar o script.

* **Windows (CMD):**  set GROQ_API_KEY=sua_chave_aqui

* **Windows (PowerShell):** $env:GROQ_API_KEY="sua_chave_aqui"

* **Linux/macOS:** export GROQ_API_KEY="sua_chave_aqui"

## Opção B (Direto no Código): Abra o arquivo chatbot.py com um editor de texto, localize a linha abaixo e substitua o texto padrão pela sua chave:

````
Python
CHAVE_API = os.environ.get("GROQ_API_KEY", "SUA_CHAVE_AQUI_ENTRE_AS_ASPAS")
````
Passo 4: Executar o Chatbot
**Com a biblioteca instalada** e a chave configurada, inicie o programa rodando o comando:

````
Bash
python chatbot.py
````
## Passo 5: Interagir e Sair
Digite suas dúvidas no terminal e pressione Enter para receber a resposta do bot.

Para encerrar o chat a qualquer momento, digite sair, quit ou exit e pressione Enter.
