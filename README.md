# 💻 max1337xyz — Portfólio Terminal

Site de portfólio pessoal com estética **retrô / hacker**, simulando uma janela de terminal Linux com efeito de monitor CRT. Feito apenas com **HTML5, CSS3 e JavaScript puro**, sem frameworks e sem build.

```
guest@max1337xyz:~$ cat about.txt
```

## ✨ Funcionalidades

- **Tela de boot** estilo BIOS/Linux (pode ser pulada com clique, tecla ou botão)
- **Efeito CRT**: scanlines, vinheta, leve cintilação e brilho de fósforo nos textos
- **Efeito typewriter** com cursor piscante nos textos principais
- **Terminal interativo** com comandos funcionais e histórico (↑ / ↓)
- **Janela de terminal** com botões de minimizar, maximizar e fechar
- **Cards de projetos** estilizados como diretórios/arquivos (`ls -la`)
- **Barras de skills** animadas
- **Botões de copiar** e-mail e telefone, com aviso na tela
- **Hover invertido** (fundo verde, texto preto) em links e botões
- **100% responsivo**: o banner ASCII escala com a largura da tela
- Respeita `prefers-reduced-motion`

## 🖥️ Comandos do terminal

| Comando    | O que faz                                      |
|------------|------------------------------------------------|
| `help`     | Lista os comandos disponíveis                  |
| `about`    | Resumo e rola até a seção Sobre                |
| `projects` | Lista os projetos e rola até a seção           |
| `skills`   | Mostra as skills e rola até a seção            |
| `contact`  | Mostra os contatos e rola até a seção          |
| `github`   | Abre o perfil do GitHub em nova aba            |
| `whoami`   | Quem é você (e quem é o dono do site)          |
| `date`     | Data e hora atuais                             |
| `ls`       | Lista os "arquivos" do site                    |
| `clear`    | Limpa o terminal                               |
| `sudo`     | Surpresa 😉                                    |

## 📁 Estrutura

O projeto inteiro é **um único arquivo**, com CSS e JS embutidos e comentados por seção:

```
.
├── portfolio.html   # renomeie para index.html ao publicar
└── README.md
```

## 🚀 Como usar

### Localmente

Baixe o arquivo e abra no navegador. Não precisa de servidor nem de dependências.

```bash
git clone https://github.com/max1337xyz/<nome-do-repositorio>.git
cd <nome-do-repositorio>
xdg-open index.html   # Linux
```

### Publicar no GitHub Pages

1. Renomeie `portfolio.html` para `index.html`
2. Envie para um repositório no GitHub
3. Vá em **Settings → Pages**
4. Em **Source**, escolha a branch `main` e a pasta `/ (root)`
5. O site ficará disponível em `https://max1337xyz.github.io/<nome-do-repositorio>/`

> Dica: se o repositório se chamar `max1337xyz.github.io`, o site abre direto em `https://max1337xyz.github.io`.

## 🛠️ Personalização

| O que alterar            | Onde                                                              |
|--------------------------|-------------------------------------------------------------------|
| Cores e fontes           | Variáveis em `:root` no início do `<style>`                       |
| Texto da seção Sobre     | `<section id="sobre">`                                            |
| Projetos                 | Cards em `<section id="projetos">` (procure os comentários `PLACEHOLDER`) |
| Skills e porcentagens    | Array `SKILLS` no `<script>`                                      |
| Contatos                 | `<section id="contato">` e o comando `contact` em `CMDS`          |
| Texto do boot            | Array `BOOT` no `<script>`                                        |
| Nickname do banner ASCII | String `"max1337xyz"` na geração do banner (letras disponíveis: `m a x 1 3 7 y z`; para outras letras, adicione-as ao objeto `F`) |

### Adicionando um novo projeto

Copie um card existente e edite título, descrição, tags e link:

```html
<article class="card">
  <span class="perm">drwxr-xr-x  max1337xyz</span>
  <h3>📁 nome-do-projeto</h3>
  <p>Descrição curta do projeto.</p>
  <div class="tags"><span class="tag">Python</span></div>
  <a href="https://github.com/max1337xyz/nome-do-projeto" target="_blank" rel="noopener noreferrer">[ ver repositório ↗ ]</a>
</article>
```

## 🧰 Tecnologias

- HTML5 semântico
- CSS3 (Grid, Flexbox, variáveis CSS, animações)
- JavaScript (Vanilla JS)
- Fontes [Fira Code](https://fonts.google.com/specimen/Fira+Code) e [VT323](https://fonts.google.com/specimen/VT323) via Google Fonts

## ⚠️ Aviso sobre projetos de segurança

O projeto em destaque, `Phishing-Script-Kali-Linux`, é voltado a **estudos de cibersegurança e testes de engenharia social em ambientes autorizados**. Use ferramentas desse tipo apenas com permissão explícita e de forma ética e legal.

## 📬 Contato

- GitHub: [github.com/max1337xyz](https://github.com/max1337xyz)
- E-mail: [dlcninnja12@gmail.com](mailto:dlcninnja12@gmail.com)
- WhatsApp: [(85) 92002-0969](https://wa.me/5585920020969)

## 📄 Licença

Defina a licença de sua preferência (por exemplo, [MIT](https://choosealicense.com/licenses/mit/)).
