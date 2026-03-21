# ⭐ Arena App

PWA para organizar peladas, campeonatos e partidas de raquete.

## Funcionalidades

- **⚽ Pelada** — seleciona jogadores, sorteia times equilibrados por nível, cronômetro, placar, log de gols e assistências
- **🎾 Beach Tennis / 🏓 Padel / 🎾 Tênis** — placar oficial (0-15-30-40-Deuce-Adv, games, sets, tiebreak)
- **🏆 Ranking** — artilheiros, assistentes e vencedores
- **📋 Histórico** — resumo semanal e histórico completo
- **📲 PWA** — instala no celular, funciona offline

---

## Como subir no GitHub Pages

### 1. Crie um repositório no GitHub

```bash
# Na sua máquina, dentro da pasta arena-app:
git init
git add .
git commit -m "Arena App v1"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/arena-app.git
git push -u origin main
```

### 2. Ative o GitHub Pages

1. Vá em **Settings** do repositório
2. Clique em **Pages** no menu lateral
3. Em **Branch**, selecione `main` e pasta `/` (root)
4. Clique **Save**
5. Aguarde ~1 minuto

### 3. Acesse o app

O app estará disponível em:
```
https://SEU_USUARIO.github.io/arena-app/
```

### 4. Instalar no celular

**Android (Chrome):**
- Acesse a URL acima
- Toque nos 3 pontinhos → "Adicionar à tela inicial"

**iPhone (Safari):**
- Acesse a URL no Safari
- Toque em Compartilhar (quadrado com seta) → "Adicionar à Tela de Início"

---

## Estrutura dos arquivos

```
arena-app/
  index.html    ← App completo (HTML + CSS + JS)
  manifest.json ← Configuração PWA
  sw.js         ← Service Worker (offline)
  README.md     ← Este arquivo
```

---

## Tecnologias

- HTML5 / CSS3 / JavaScript puro
- PWA (Progressive Web App)
- localStorage para persistência local
- Nenhuma dependência externa

---

## Personalização

Para mudar os nomes dos times padrão, edite em `index.html`:
```js
document.getElementById('fname-0').textContent = 'SEU TIME';
```

Para mudar a duração padrão dos jogos:
```js
let peladaCfg = { ..., duration: 10 }  // 10 minutos
```
