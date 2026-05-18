# 🤖 Chatbot com Inteligência Artificial (Llama 3)

Este projeto é um programa simples que cria um chat de conversa no seu computador. Ele usa a tecnologia da Groq (uma plataforma super rápida) e o modelo Llama 3 (uma inteligência artificial parecida com o ChatGPT) para responder suas perguntas direto pelo terminal de comandos. Ele se adapta ao Usuario para aprender sobre ele e realizar conselhos baseados no usuario

O grande diferencial deste robô é que ele foi programado para ser amigável com iniciantes, ético nas respostas e capaz de lembrar o que você conversou com ele durante a sessão.

---

## 🛠️ O que você precisa antes de começar

Para que o código funcione, você precisa ter apenas duas coisas:
1. **Python instalado:** É a linguagem de programação usada para rodar o projeto. Se não tiver, baixe e instale a versão mais recente pelo site oficial (python.org).
2. **Uma chave da Groq (API Key):** É como uma senha que permite que o seu código converse com os servidores de inteligência artificial. Você consegue uma criando uma conta gratuita no site [Groq Cloud](https://console.groq.com/).

---

## 🏁 Passo a Passo para Rodar o Programa

Siga estas instruções simples para colocar o seu robô para funcionar:

### Passo 1: Salvar o arquivo do projeto
1. Abra o bloco de notas do seu computador.
2. Copie todo o código em Python do chatbot e cole dentro do bloco de notas.
3. Salve o arquivo com o nome `chatbot.py` em uma pasta de sua preferência (por exemplo, na Área de Trabalho).

### Passo 2: Abrir o Terminal na pasta correta
1. Abra o **Prompt de Comando** (se usar Windows) ou o **Terminal** (se usar Mac ou Linux).
2. Você precisa navegar até a pasta onde salvou o arquivo. Se salvou na Área de Trabalho do Windows, por exemplo, digite o comando abaixo e aperte Enter:
   ```bash
   cd Desktop
   ```
### Passo 3: Instalar o conector da Groq
O Python precisa de um pacote especial para conseguir conversar com a inteligência artificial da Groq. Para instalar esse pacote, digite o comando abaixo no seu terminal e aperte Enter:

```
Bash
pip install groq
```
Aguarde alguns segundos até aparecer uma mensagem dizendo que a instalação foi concluída com sucesso.

### Passo 4: Colocar a sua chave de acesso no código
Para o robô funcionar, você precisa colar a chave (senha) que pegou no site da Groq dentro do seu arquivo.

Abra o arquivo chatbot.py no bloco de notas.

Procure pela linha número 12, que se parece com isso:

```
Python
CHAVE_API = os.environ.get("GROQ_API_KEY", "COLOQUE_SUA_CHAVE_API_AQUI")
```
Apague o texto COLOQUE_SUA_CHAVE_API_AQUI e cole a sua chave gerada no site da Groq ali dentro, mantendo as aspas. Vai ficar mais ou menos assim:

```
Python
CHAVE_API = os.environ.get("GROQ_API_KEY", "gsk_a1B2c3D4e5...")
```
Salve e feche o arquivo.

### Passo 5: Iniciar a conversa!
Agora está tudo pronto. Para abrir o seu chat, digite o comando abaixo no terminal e aperte Enter:

```Bash
python chatbot.py
```
### Pronto! 

* O terminal vai mostrar uma mensagem de boas-vindas.

* Para conversar: Digite o que quiser e aperte Enter para ver a resposta do robô.

* Para fechar o programa: Quando cansar de conversar, basta digitar a palavra sair e apertar Enter.
