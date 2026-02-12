# TMachine-Intelig-ncia-Artificial-[README.md](https://github.com/user-attachments/files/25266276/README.md)
# 🎮 Pedra, Papel e Tesoura com IA

## 📝 Descrição
Jogo de Pedra, Papel e Tesoura que usa reconhecimento de gestos com IA treinada no Teachable Machine do Google. Você faz os gestos com a mão na webcam e joga contra o computador!

## 🚀 Como Usar

### Passo 1: Treinar o Modelo no Teachable Machine
1. Acesse [Teachable Machine](https://teachablemachine.withgoogle.com/)
2. Clique em **"Get Started"**
3. Escolha **"Image Project"** → **"Standard image model"**
4. Renomeie as 3 classes para:
   - **Pedra** (punho fechado ✊)
   - **Papel** (mão aberta ✋)
   - **Tesoura** (dedos em V ✌️)
5. Para cada classe, clique em **"Webcam"** e capture pelo menos **30-50 fotos** do gesto
   - Varie a posição da mão, ângulos, distância
   - Fundo neutro ajuda!
6. Clique em **"Train Model"** (vai demorar alguns minutos)
7. Teste o modelo na aba **"Preview"**
8. Clique em **"Export Model"**
9. Escolha a aba **"Upload (shareable link)"**
10. Clique em **"Upload my model"**
11. **Copie a URL gerada** (algo como `https://teachablemachine.withgoogle.com/models/xxxxx/`)

### Passo 2: Executar a Aplicação

#### Opção A: Abrir Localmente
1. Baixe o arquivo `index.html`
2. Dê duplo-clique no arquivo (abre no navegador)
3. Cole a URL do modelo que você copiou
4. Clique em **"Carregar Modelo e Iniciar Webcam"**
5. Permita acesso à webcam quando solicitado
6. Faça os gestos e clique em **"JOGAR!"**

#### Opção B: Hospedar no GitHub Pages
1. Crie um repositório no GitHub
2. Faça upload do arquivo `index.html`
3. Vá em **Settings** → **Pages**
4. Em **Source**, escolha a branch `main` e pasta `/ (root)`
5. Clique em **Save**
6. Acesse a URL gerada (ex: `https://seu-usuario.github.io/nome-repo/`)

#### Opção C: Usar um servidor local
```bash
# Se você tem Python instalado:
python -m http.server 8000
# Acesse: http://localhost:8000
```

## 🎯 Como Jogar
1. Após carregar o modelo, você verá a webcam e as predições em tempo real
2. Posicione sua mão na frente da webcam fazendo um dos gestos
3. Quando estiver pronto, clique em **"JOGAR!"**
4. O computador escolhe aleatoriamente e o resultado aparece!
5. O placar é atualizado automaticamente

## 🛠️ Tecnologias Utilizadas
- **HTML5/CSS3/JavaScript** (puro, sem frameworks)
- **TensorFlow.js** - Para executar o modelo de IA
- **Teachable Machine Library** - Interface com modelos do Teachable Machine
- **WebRTC** - Para acesso à webcam

## 📋 Requisitos
- Navegador moderno (Chrome, Firefox, Edge)
- Webcam funcional
- Conexão com internet (para carregar bibliotecas)
- Permissão de acesso à webcam

## 🎨 Features
- ✅ Interface visual bonita e responsiva
- ✅ Predições em tempo real com barras de confiança
- ✅ Placar de vitórias/derrotas/empates
- ✅ Animações suaves
- ✅ Instruções passo a passo incluídas
- ✅ Totalmente funcional em arquivo único (fácil de compartilhar)

## 💡 Dicas para Melhores Resultados
- Treine o modelo com boa iluminação
- Use um fundo neutro ou consistente
- Capture variações do gesto (diferentes ângulos, distâncias)
- Teste bem o modelo antes de exportar
- Se a detecção não estiver boa, treine com mais imagens

## 🐛 Solução de Problemas

**Webcam não funciona:**
- Verifique se deu permissão ao navegador
- Tente outro navegador (Chrome funciona melhor)
- Verifique se nenhum outro app está usando a webcam

**Modelo não carrega:**
- Verifique se a URL está completa e correta
- Certifique-se que fez o upload no Teachable Machine
- Tente gerar uma nova URL

**Detecção imprecisa:**
- Treine com mais imagens (100+ por classe é ideal)
- Varie mais os ângulos durante o treino
- Certifique-se que as condições de luz são similares

## 📄 Licença
Projeto educacional livre para uso em sala de aula.

