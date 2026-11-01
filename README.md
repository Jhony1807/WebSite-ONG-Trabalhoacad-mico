TRABALHO ACADÊMICO - DESENVOLVIMENTO FRONT END | ONG E-sports Projeto final
# Instituto Level Up Periferia — Projeto Integrador (ONG)

Site de uma ONG **fictícia** que prepara crianças e jovens da periferia de São Paulo para o cenário dos e-sports (Counter-Strike 2 e Valorant). Feito com HTML5, CSS3 e JavaScript puro, sem frameworks e sem backend.

> Projeto acadêmico da disciplina de Desenvolvimento Front-end, do professor Marcelo de Freitas Pintaud. Nenhum dado é coletado ou enviado.

## Integrantes
- Jonata Alves Borsari — <a href="https://www.linkedin.com/in/jonata-alves-borsari/
- Joao Frazon Zanon — <a href=" https://www.linkedin.com/in/jo%C3%A3o-fraz%C3%A3o-zanon/>
- Gustavo Ferreira Lima — <a href="https://www.linkedin.com/in/gustavo-ferreira-b83b8b443
- Nicolas Henry Oliveira Penha — <a href="https://www.linkedin.com/in/nicolas-henry-oliveira/
- Gabriel Braes Gramacho — <a href="https://www.linkedin.com/in/gabriel-braes-gramacho-3a6191403

## Objetivo
Divulgar a causa, apresentar os projetos, explicar os jogos e receber inscrições (simuladas).

## Páginas
| Página | O que tem |
|---|---|
| `index.html` | Início: destaque, números de impacto e aviso de projeto acadêmico |
| `sobre.html` | História, missão, **contribuições**, público atendido, lan house com fotos lado a lado, objetivos e botão JS de informações institucionais |
| `projetos.html` | Três cartões de projetos com "Como contribuir" e botão **Quero participar** centralizado embaixo |
| `cs2.html` | Counter-Strike 2 (tema laranja): história ampliada e "Como se joga" em tópicos |
| `valorant.html` | Valorant (tema vermelho/marinho): história ampliada e "Como se joga" em tópicos |
| `contato.html` | Formulário de inscrição com validação em JavaScript |


### HTML
- Código reorganizado e indentado (4 espaços), com `<section>`, `<div>`, `<h1>`, `<h2>` e comentários de COMMIT em cada bloco.
- Tags que ficavam abertas foram corrigidas: `<div>` em `sobre.html` e `projetos.html` e `<p>` dos parceiros no rodapé de todas as páginas.
- Menu na mesma ordem em todas as páginas: Início, Sobre, Projetos, CS2, Valorant, Contato. Cada página marca apenas a si mesma como página atual.
- **projetos.html:** o botão "Quero participar" saiu de dentro da fileira de cartões e ficou centralizado abaixo deles. Os textos "Como contribuir" ficam alinhados no fim de cada cartão.
- **sobre.html:** estrutura em duas colunas (história e missão de um lado, público atendido do outro), seção "Contribuímos" e fotos da lan house em `<figure>` com legenda. Também corrigido o texto do botão, que estava com espaços sobrando.
- **cs2.html e valorant.html:** a seção "A história" ganhou mais contexto (origem do jogo, chegada ao Brasil, cenário competitivo) e "Como se joga" virou lista com tópicos em negrito (equipes, objetivo, rodadas ou vitória, agentes no Valorant e economia).

### CSS (`estilos.css`)
- `.cartao` agora usa `flex-direction: column` e `.cartao-corpo` usa `flex: 1`, para alinhar o "Como contribuir" no fim do cartão.
- Fotos dos cartões com proporção fixa (`aspect-ratio: 3 / 2` e `object-fit: cover`).
- Novo bloco `.figuras` (grade de 2 colunas, 1 coluna no celular) para fotos lado a lado com legenda.
- Nova classe `.acoes.centro` para centralizar botões.

### JavaScript
1. `formulario.js`: validação do formulário (`submit`, `preventDefault`, `trim`, mensagens de erro e confirmação simulada). A primeira regra avisa quando há **campos obrigatórios vazios**; depois vêm as regras específicas, na ordem: nome (mínimo de 3 caracteres), e-mail válido, jogo escolhido e mensagem (mínimo de 10 caracteres).
2. `script.js`: botão mostrar/ocultar informações institucionais em `sobre.html`.

## Estrutura
```
index.html  sobre.html  projetos.html  cs2.html  valorant.html  contato.html
estilos.css  formulario.js  script.js  README.md
img/  (imagens do site)
```

## Como executar
Abra `index.html` no navegador. Não precisa de instalação.

## Imagens e créditos
Arquivos locais usados em `img/`: `campeonato-cs2.webp`, `treinando.webp`, `time-jogando.webp`, `jogador-fones.webp`, `disputa.webp` e `valorant-fone.webp`.

Algumas imagens ainda são carregadas de links externos. O ideal é baixá-las para `img/` e trocar o `src`, para não depender de outros sites.

| Uso | Origem | Autor | Licença |
|---|---|---|---|
| Cartão "Jogador Estudante" (`projetos.html`) | catracalivre.com.br (imagem de Stefan Meller, Pixabay) | (preencher) | (preencher) |
| Cartão "Liga da Quebrada" (`projetos.html`) | media.maisesports.com.br (IEM Rio 2022, Stephanie Lindgren) | (preencher) | (preencher) |
| Lan house (`sobre.html`) | Google Imagens | (preencher) | (preencher) |
| Jogadores na ESWC 2010 (`sobre.html`) | millenium.gg (foto HLTV) | (preencher) | (preencher) |
| Ícone do CS2 (`cs2.html`) | dashboard-icons (homarr-labs) | (preencher) | (preencher) |
| Ícone do Valorant (`valorant.html`) | dashboardicons.com (Simple Icons) | (preencher) | (preencher) |
| Imagens em `img/` | (preencher) | (preencher) | (preencher) |

Fontes: Google Fonts (Barlow Condensed e Nunito Sans). Counter-Strike 2 e Valorant são marcas de seus donos (Valve e Riot Games); o projeto é acadêmico e não é oficial.
