# Skills de design/frontend para agentes de IA

> Fonte: reel do Instagram https://www.instagram.com/reel/DeWZ41iTdpE/ (pt-BR, com legenda "Comenta DESIGN que eu te mando as 5 ferramentas de design pro Claude Code").
> Tema: deixar sites/apps gerados por agentes (Claude Code, Cursor, Copilot) com uma cara menos genérica.
> Os links abaixo são os que aparecem na tela do vídeo; o vídeo não explica como instalar cada uma.

---

## 1. Taste Skill

- **O que faz:** ensina o agente a ter "bom gosto" em design e a fugir de layouts repetitivos (o exemplo do vídeo é o "degradê roxo com 3 cards arredondados").
- **Descrição mostrada no vídeo:** "The anti-slop frontend framework for AI agents. Open-source text files that drive Claude Code, Cursor, Copilot, and other coding agents towards premium..."
- **Como usar:** adicione os arquivos de texto da skill ao projeto ou ao agente, para que ele siga essas diretrizes quando gerar interfaces.
- **Link:** [tasteskill.dev](https://tasteskill.dev)

## 2. Web Design Guidelines (`web-design-guidelines`)

- **O que faz:** audita a interface que o agente já construiu, comparando com regras de design. Confere contraste do texto, espaçamento, hierarquia, alinhamento e foco dos botões.
- **Como usar:** peça ao agente uma auditoria da UI pronta com essa skill e depois corrija o que ela apontar.
- **Link:** [skills.sh](https://skills.sh)

## 3. Awesome Design (`awesome-design-md`)

- **O que faz:** é uma coleção de arquivos `DESIGN.md` baseados em design systems de marcas conhecidas. Dá ao agente referências reais de tipografia, cor, espaçamento, componentes e layout.
- **Descrição mostrada no vídeo:** "A collection of DESIGN.md files analysis by popular brand design systems. Drop one into your project and let coding agents generate a matching UI."
- **Como usar:** coloque um `DESIGN.md` no projeto e peça ao agente para gerar a UI seguindo esse arquivo.
- **Link:** [getdesign.md](https://getdesign.md)

## 4. Image to Code

- **O que faz:** recria em código um design tirado de uma imagem ou print, por exemplo uma referência do Pinterest.
- **Como usar:** tire um print do design que você gosta, mande para o agente e peça para ele reproduzir a tela.
- **Link:** no vídeo aparece só "github.com", sem o repositório exato.

## 5. Playwright CLI (`playwright-cli`)

- **O que faz:** deixa o agente abrir o navegador, interagir com o site que ele gerou, tirar screenshots e conferir visualmente o próprio trabalho.
- **Descrição mostrada no vídeo:** "CLI for common Playwright actions. Record and generate Playwright code, inspect selectors and take screenshots."
- **Como usar:** depois de gerar a tela, o agente roda o Playwright para abrir a página, tirar prints e corrigir o que estiver errado.
- **Link:** [playwright.dev](https://playwright.dev)

---

## Fluxo sugerido

1. Use a **Taste Skill** e um **awesome-design-md** como base de estilo.
2. Se tiver uma referência visual, use o **Image to Code**.
3. Rode o **Playwright CLI** para o agente ver o resultado.
4. Feche com uma auditoria usando o **web-design-guidelines**.
