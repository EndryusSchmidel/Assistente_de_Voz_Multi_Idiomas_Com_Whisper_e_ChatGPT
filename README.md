# 🎙️ Assistente de Voz com ChatGPT e Whisper

Projeto desenvolvido durante o Bootcamp Bradesco - Java Cloud Native na DIO. O sistema captura áudio, transcreve usando IA, processa a resposta e a converte novamente em voz.

## 🛠️ Tecnologias Utilizadas
* **Python**
* **OpenAI Whisper**: Transcrição de áudio (Speech-to-Text).
* **OpenAI GPT-3.5/4**: Processamento de linguagem natural.
* **gTTS (Google Text-to-Speech)**: Síntese de voz (Text-to-Speech).

## 🚀 Como Funciona
1. O áudio é gravado via JavaScript no navegador.
2. O modelo **Whisper** converte o áudio `.wav` em texto.
3. O texto é enviado para a API da OpenAI.
4. A resposta retorna e é convertida em um arquivo de áudio pelo **gTTS**.

> **Nota técnica:** Durante o desenvolvimento, integrei uma lógica de tratamento para limites de cota de API, garantindo que o fluxo de conversão de voz (TTS) fosse validado mesmo em modo de simulação.
