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

speakview/
├── app/
│ ├── audio/ # Captura de microfone e áudio do sistema
│ ├── transcriber/ # Módulo de transcrição com Whisper
│ ├── storage/ # Banco de dados local (SQLite)
│ ├── ui/ # Interface gráfica
│ └── main.py # Arquivo principal da aplicação
├── assets/ # Ícones, fontes, imagens
├── requirements.txt # Bibliotecas Python
├── Dockerfile # Docker container
├── docker-compose.yml # Subida do app com Docker
└── README.md

yaml
Copiar
Editar

---

## 🐳 Como rodar com Docker

### 1. Clonar o repositório

bash
git clone https://github.com/thiagosimi10/speakview.git
cd speakview
2. Configurar variáveis de ambiente
Crie um arquivo .env com sua chave da OpenAI:

env
Copiar
Editar
OPENAI_API_KEY=sk-xxxxx
3. Rodar com Docker
bash
Copiar
Editar
docker-compose up --build
Isso irá criar o container, instalar as dependências e iniciar a aplicação com interface gráfica.

⚠️ Requisitos para Captura de Áudio do Sistema
Para capturar o áudio da reunião (saída do sistema):

Windows
Instale VB-Cable

Configure o cabo virtual como dispositivo de saída padrão

macOS
Use o BlackHole

Linux
Configure loopback com pavucontrol ou alsa

🧪 Em breve
🧑‍💼 Identificação de locutor (diarização)

📄 Exportação para PDF

📝 Resumo automático da reunião

☁️ Integração com serviços como Google Drive

📄 Licença
Distribuído sob a licença MIT. Veja o arquivo LICENSE para mais informações.

🤝 Contribuições
Pull requests são bem-vindos! Sinta-se à vontade para abrir issues, sugerir melhorias ou colaborar com novas features.

👨‍💻 Autor
Desenvolvido por Thiago Simionato com o apoio da IA.



