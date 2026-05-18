# 🤖 Chatbot com Inteligência Artificial (Llama 3)

Este projeto é um programa simples que cria um chat de conversa no seu computador. Ele usa a tecnologia da Groq (uma plataforma super rápida) e o modelo Llama 3 (uma inteligência artificial parecida com o ChatGPT) para responder suas perguntas direto pelo terminal de comandos. Ele se adapta ao Usuario para aprender sobre ele e realizar conselhos baseados no usuario

O grande diferencial deste robô é que ele foi programado para ser amigável com iniciantes, ético nas respostas e capaz de lembrar o que você conversou com ele durante a sessão.

---

## 🛠️ O que você precisa antes de começar

Para que o código funcione, você precisa de apenas duas coisas:
1. **Uma chave da Groq (API Key):** É como uma senha que permite que o seu código converse com os servidores de inteligência artificial. Você consegue uma criando uma conta gratuita no site [Groq Cloud](https://console.groq.com/).
2. **Escolher onde vai rodar:** Você pode rodar este projeto direto no seu navegador usando o **Google Colab** (sem precisar instalar nada no PC) ou direto no **Windows**.

---

## 🏁 Como Usar no Google Colab (Pelo Navegador)

O Google Colab é a forma mais fácil se você não quer instalar o Python no seu computador.

1. Acesse o [Google Colab](https://colab.research.google.com/) e crie um **Novo Notebook**.
2. Na primeira célula de código, instale a biblioteca da Groq digitando o comando abaixo e clicando no botão de "Play":
   ```python
   !pip install groq
---

* Crie uma nova célula de código, cole todo o código em Python do seu chatbot.

* Antes de apertar o "Play", mude a linha 12 do código, colocando a sua chave da Groq no lugar do texto padrão, assim:

```
Python
CHAVE_API = os.environ.get("GROQ_API_KEY", "SUA_CHAVE_AQUI_DA_GROQ")
```

* Clique no botão de "Play" para rodar. O chat vai abrir logo abaixo da célula. Digite suas perguntas e, quando quiser parar, digite sair.

###🏁 Como Usar no Windows (Direto no Computador)
Se preferir rodar direto na sua máquina Windows, siga estes passos:

## Passo 1: Ter o Python instalado
Certifique-se de ter o Python instalado no seu Windows. Você pode baixá-lo na Microsoft Store ou pelo site oficial (python.org). Marque a opção "Add Python to PATH" durante a instalação.

## Passo 2: Salvar o arquivo do projeto
Abra o Bloco de Notas do Windows.

Copie todo o código em Python do chatbot e cole dentro dele.

Vá em Arquivo > Salvar Como. Escolha uma pasta (como a Área de Trabalho), mude o tipo para "Todos os arquivos (.)" e salve com o nome chatbot.py.

## Passo 3: Colocar a sua chave de acesso no código
No arquivo chatbot.py que você acabou de salvar, procure pela linha 12:

```
Python
CHAVE_API = os.environ.get("GROQ_API_KEY", "COLOQUE_SUA_CHAVE_API_AQUI")
````
* Apague o texto COLOQUE_SUA_CHAVE_API_AQUI e cole a sua chave gerada no site da Groq ali dentro, mantendo as aspas. Exemplo:

```
Python
CHAVE_API = os.environ.get("GROQ_API_KEY", "gsk_a1B2c3D4e5...")
```
* Salve e feche o arquivo.

## Passo 4: Abrir o Prompt de Comando e Instalar a biblioteca
*Abra o menu iniciar do Windows, digite CMD (Prompt de Comando) e abra-o.

*Navegue até a pasta onde salvou o arquivo. Se foi na Área de Trabalho, digite:

```
DOS
cd Desktop
```
* Instale o conector da Groq digitando o comando abaixo e apertando Enter:

```
DOS
pip install groq
```
## Passo 5: Iniciar a conversa!
* Para abrir o seu chat no Windows, digite o comando abaixo no terminal e aperte Enter:

```
DOS
python chatbot.py
```
### Pronto! 
* vO terminal vai mostrar que o chat foi iniciado.

* Para conversar: Digite sua mensagem e aperte Enter.

* Para fechar o programa: Quando quiser encerrar, digite a palavra sair e aperte Enter.
