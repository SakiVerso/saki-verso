# Saki Verso: Lâmina Neon

Side-scroller 2D inspirado em Rygar, feito em HTML5 Canvas e JavaScript puro. Cinco fases, cinco chefes e um Super Boss final. Joga com teclado ou controle, direto no navegador. Sem instalação e sem dependências.

> Onde o Mundo Gamer e Tecnologia estão sempre On

https://saki-verso-saki-verso.vercel.app

## O jogo

Você é a Saki Verso. Atravesse as fases, derrote os chefes e enfrente o Soberano do Núcleo, o Super Boss, que luta em duas fases.

| Fase | Mundo | Chefe |
|---|---|---|
| 1 | Floresta Neon | Guardião de Pedra |
| 2 | Castelo Arruinado | Verme Cristalino |
| 3 | Cemitério Assombrado | Andróide Defeituoso |
| 4 | Salão do Trono Corrompido | Cavaleiro Sombrio |
| 5 | O Núcleo do Mal | Soberano do Núcleo (Super Boss) |

### Controles

| Ação | Teclado | Controle |
|---|---|---|
| Mover | Setas ou A / D | Direcional ou analógico |
| Pular | Espaço, W ou ↑ | ✕ |
| Espada | X ou J | □ |
| Shuriken | Z ou K | ○ ou R1 |
| Shuriken para cima | C ou L | △ |
| Especial (barra cheia) | E ou Shift | L1 |
| Pausa | P ou Esc | Start |
| Som ligado/desligado | M | |
| Tela cheia | F | |

## Estrutura do projeto

```
index.html   página do site (visual neon, jogo, fases e área de contribuição)
style.css    estilo do site
game.js      todo o jogo (lógica, áudio, fases, chefes) e os sprites embutidos
README.md    este guia
```

O site é estático: não precisa de build. Para testar no computador, basta abrir o `index.html` no navegador.

---

## Publicar o site (passo a passo, sem terminal)

### 1. Colocar os arquivos no GitHub

1. Crie uma conta em github.com e entre.
2. Clique em **New** (botão verde, canto superior esquerdo) para criar um repositório.
3. Em **Repository name**, escreva `saki-verso`. Deixe **Public** marcado.
4. Marque **Add a README file** e também **Choose a license** com **MIT License** (vale para o código).
5. Clique em **Create repository**.
6. Na página do repositório, clique em **Add file → Upload files** e arraste `index.html`, `style.css` e `game.js`. Para o `README.md`, faça o mesmo e confirme a substituição.
7. Clique em **Commit changes**.

### 2. Ligar o repositório à Vercel

1. Entre em vercel.com com **Continue with GitHub**.
2. Clique em **Add New → Project**.
3. Ache `saki-verso` na lista e clique em **Import**.
4. Em **Framework Preset**, deixe **Other**. Não mude mais nada.
5. Clique em **Deploy** e espere cerca de um minuto. A Vercel mostra o endereço do site.

### 3. Usar seu endereço próprio (opcional)

No projeto da Vercel, abra **Settings → Domains**, digite o domínio e siga as instruções que aparecem na tela.

### 4. Atualizar o site depois

1. No GitHub, abra o arquivo que quer mudar e clique no ícone de lápis.
2. Edite e clique em **Commit changes**.
3. Pronto: a Vercel publica a nova versão sozinha em cerca de um minuto.

### 5. Ativar Issues e Discussions

No repositório, abra **Settings**, role até **Features** e marque **Issues** e **Discussions**. Assim os botões da área de contribuição funcionam.

---

## Como contribuir

Toda ajuda é bem-vinda: bugs, ideias de inimigos, novas fases, balanceamento, melhorias de som e visual.

1. **Reportar bug ou sugerir ideia:** abra uma Issue ou uma Discussion e descreva o caso. Diga a fase e se usava teclado ou controle.
2. **Enviar uma melhoria:**
   1. Clique em **Fork** no topo do repositório.
   2. No seu fork, edite os arquivos (lápis) e clique em **Commit changes**.
   3. Volte à página do seu fork e clique em **Contribute → Open pull request**.
   4. Explique o que mudou e por quê.
3. Antes de enviar, abra o `index.html` e jogue ao menos uma fase para conferir que nada quebrou.

### Dicas para quem mexe no `game.js`

- A linha 1 contém os sprites em base64 (`const DATA`). Não edite essa linha; o código do jogo começa na linha 2.
- As fases ficam em `STAGES`. Cada uma define nome, chefe, cores, vida do chefe e comportamento.
- A física e as colisões estão em `update()`, e o desenho em `draw()`.

## Créditos e licença

- Código do jogo: MIT. O arquivo `LICENSE` é criado pelo GitHub quando você escolhe a licença ao criar o repositório.
- Sprites da Saki, do zumbi e do esqueleto: CraftPix. Esses arquivos seguem a licença da CraftPix e **não** são cobertos pela MIT. Confira os termos antes de tornar o repositório público e mantenha o crédito.
- Música e efeitos sonoros: gerados por código no próprio jogo.
