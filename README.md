# 🎸 André & Thiago — AR Business Card

Experiência de Realidade Aumentada para cartão de visita da dupla André & Thiago.

## 📁 Estrutura do projeto

```
andre-thiago-ar/
├── index.html          ← Página principal da experiência AR
├── assets/
│   ├── logo.png        ← Logo da dupla
│   ├── video.mp4       ← Vídeo que aparece no AR
│   └── targets.mind    ← Arquivo de marcador (você vai gerar — veja abaixo)
└── README.md
```

---

## 🎯 PASSO 1 — Gerar o arquivo `targets.mind` (marcador do cartão)

Esse arquivo ensina o MindAR a reconhecer o cartão de visita.

1. Acesse: **https://hiukim.github.io/mind-ar-js/tools/compile/**
2. Clique em **"Upload Images"**
3. Faça upload da imagem do seu **cartão de visita final** (quanto mais detalhado visualmente, melhor o reconhecimento)
4. Clique em **"Start"** e aguarde processar
5. Clique em **"Export"** → vai baixar um arquivo `targets.mind`
6. Coloque esse arquivo dentro da pasta `assets/`

> ⚠️ **Importante:** Use a imagem final do cartão impresso. A arte precisa ter bom contraste e detalhes visuais (o logo da dupla funciona muito bem como marcador!).

---

## 🚀 PASSO 2 — Subir no Vercel (gratuito)

### Opção A — Via GitHub (recomendado)

1. Crie uma conta em **github.com** (se não tiver)
2. Crie um repositório novo: `andre-thiago-ar`
3. Suba todos os arquivos da pasta do projeto
4. Acesse **vercel.com** → "Add New Project"
5. Conecte seu GitHub e selecione o repositório
6. Clique em **Deploy** — pronto! 🎉

### Opção B — Via Vercel CLI

```bash
npm i -g vercel
cd andre-thiago-ar
vercel
```

---

## 📱 PASSO 3 — Gerar o QR Code

Após o deploy, você vai ter uma URL tipo:
`https://andre-thiago-ar.vercel.app`

1. Acesse **qr.io** ou **qrcode-monkey.com**
2. Cole a URL
3. Customize com as cores da dupla (verde escuro + dourado)
4. Baixe em alta resolução para colocar no cartão

---

## 🃏 PASSO 4 — O cartão de visita

Sugestão de layout para o cartão:
- **Frente:** Logo da dupla + redes sociais
- **Verso:** Logo menor + QR Code + instrução: *"Aponte a câmera aqui e veja a mágica!"*

Ferramentas para criar o cartão:
- **Canva** (canva.com) — mais fácil
- **Figma** — mais controle

---

## 🔧 Como funciona

1. Pessoa recebe o cartão
2. Aponta a câmera do celular para o cartão (não precisa de app!)
3. O browser abre automaticamente via QR Code
4. MindAR reconhece o cartão e dispara o vídeo em cima dele
5. O vídeo de vocês tocando aparece "saindo" do cartão em AR 🎸

---

## 📞 Suporte

Instagram: [@andreethiago19](https://www.instagram.com/andreethiago19)
