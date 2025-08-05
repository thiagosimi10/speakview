# 🎙️ SpeakView

**SpeakView** é um aplicativo em Python para transcrição de voz em tempo real durante reuniões no Teams, Google Meet e outras plataformas. Ele escuta tanto seu microfone quanto o áudio da reunião, transcreve o que é dito com tecnologia de IA, e exibe tudo em uma interface clara e moderna.

> 🔧 Projeto open-source e extensível, com backend em Python e integração com modelos de transcrição (como Whisper).

---

## 📸 Demonstração (em breve)

⚠️ *GIF ou screenshot será adicionado após MVP.*

---

## 🚀 Funcionalidades

- 🎧 Captura de áudio do **microfone** e do **sistema**
- 🧠 Transcrição de voz usando **OpenAI Whisper** (API ou local)
- 📺 Exibição da transcrição em **tempo real**
- 💾 Histórico salvo em banco de dados local (SQLite)
- 🖥️ Interface gráfica com visual moderno (via `customtkinter`)
- 🐳 Pronto para rodar com **Docker**

---

## 🛠️ Tecnologias Utilizadas

- Python 3.10+
- Docker + Docker Compose
- [OpenAI Whisper](https://platform.openai.com/docs/guides/speech-to-text)
- sounddevice / PyAudio (áudio)
- SQLite (armazenamento local)
- customtkinter (GUI moderna)

---

## 📂 Estrutura do Projeto

