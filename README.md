# Arena Clash

Jogo de luta de plataforma para até 4 jogadores no mesmo dispositivo, feito em HTML5 Canvas e JavaScript puro (sem dependências, sem build).

Acumule dano (%) no rival: quanto maior o %, mais longe ele voa. Jogue-o para fora da tela para tirar uma vida.

## Como rodar

Abra o `index.html` no navegador. Não precisa de servidor.

## Como publicar no GitHub e jogar online com os amigos

```bash
git init
git add .
git commit -m "Arena Clash: primeira versão"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/arena-clash.git
git push -u origin main
```

Depois, no repositório: **Settings → Pages → Deploy from a branch → `main` / root**.
Em um minuto o jogo fica disponível em `https://SEU_USUARIO.github.io/arena-clash/`, e funciona no celular.

## Personagens

| Personagem | Armas | Força | Defesa | Veloc. | Destreza |
|---|---|---|---|---|---|
| Kael, o Duelista | Espada, Lança | 6 | 5 | 6 | 7 |
| Brutus, o Titã | Martelo, Machado | 9 | 8 | 3 | 3 |
| Lyra, a Caçadora | Arco, Manoplas | 5 | 3 | 8 | 8 |
| Zeno, o Monge | Manoplas, Lança | 6 | 4 | 9 | 6 |
| Ignis, a Berserker | Machado, Espada | 8 | 5 | 5 | 5 |
| Nyx, a Sombra | Arco, Espada | 4 | 3 | 9 | 9 |

- **Força**: dano e repulsão dos golpes
- **Defesa**: reduz a repulsão recebida
- **Velocidade**: corrida
- **Destreza**: altura do pulo e velocidade dos ataques

## Armas

Espada (equilibrada), Martelo (lento e devastador), Lança (alcance longo), Machado (pesado), Manoplas (rápidas e curtas) e Arco (projéteis).
Cada personagem carrega duas armas e troca entre elas durante a luta.

## Controles

| Esquema | Mover / pular | Leve | Pesado | Esquiva | Trocar arma |
|---|---|---|---|---|---|
| Teclado A | WASD (Espaço também pula) | J | K | L | I |
| Teclado B | Setas (Enter também pula) | , | . | / | ; |
| Teclado + Mouse | WASD, mira com o mouse | Clique esquerdo | Clique direito | Shift | E |
| Controle 1 e 2 | Analógico ou direcional, A pula | X | Y | B | LB / RB |
| Touch (celular) | Joystick virtual | LEVE | PESADO | ESQ. | TROCA |
| Bot (IA) | automático | | | | |

Segure cima ou baixo ao atacar para golpes de cima e de baixo (no ar, para baixo vira meteoro).
`Esc` volta ao menu.

## Estrutura

```
index.html   # jogo inteiro: menu, física, combate, animações, HUD e controles
README.md
```

## Ideias para evoluir

- Golpes de assinatura únicos por personagem
- Mais mapas e itens de arma que caem do céu
- Modo online (WebRTC ou WebSocket)
- Sprites e sons próprios

## Aviso

Inspirado no gênero de platform fighters (como Brawlhalla). Personagens, armas, nomes e arte são originais e o projeto não tem vínculo com a Ubisoft/Blue Mammoth.
