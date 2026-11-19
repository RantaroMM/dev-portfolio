# Marcos Barbosa — Developer Portfolio

Portfólio pessoal de **Marcos Vinicius Gomes Barbosa**, estudante de Engenharia Elétrica (ênfase em Automação e Controle) na **Poli-USP** e desenvolvedor de software com experiência em aplicações mobile, desktop, web e integração com hardware via Bluetooth Low Energy (BLE).

Site estático bilíngue (**Inglês** e **Português**), construído com **Hugo**, **Hugo Blox**, **Tailwind CSS v4** e busca local via **Pagefind**.

---

## Projetos em Destaque

- **[Gaugit (RID GAUG)](content/pt/projects/gaugit/index.md)** — Aplicativo mobile em **React Native** desenvolvido na Iniciação Científica no **IPEN**, integrado via **Bluetooth Low Energy (BLE)** ao firmware embarcado do **OpenDosimeter** para telemetria em tempo real, espectroscopia de energia (1024 canais) e configuração do detector. *Projeto premiado no X Prêmio de Inovação Tecnológica do IPEN.*
- **[Zyla](content/pt/projects/zyla/index.md)** — Aplicativo mobile de treinos e corrida desenvolvido em **React Native**, com design e estruturação das telas no **Figma**.

---

## Principais Recursos

- **Bilíngue (`EN` / `PT-BR`)**: alternância direta de idioma no cabeçalho e no rodapé (`/` e `/pt/`).
- **Tema claro/escuro**: suporte automático ao tema do sistema com tema *Dracula*.
- **Portfólio filtrável**: filtros por categoria (`Mobile`, `BLE & IoT`, `Design UI/UX`) e páginas dedicadas com capturas de tela.
- **Linha do tempo**: histórico de experiências profissionais (**BTG Pactual**, **IPEN**, **ZYLA**, **Liga de Empreendedorismo da Poli**, **Mercado Bitcoin**) e formação acadêmica na **Poli-USP**.
- **Busca integrada**: indexação estática multilíngue com **Pagefind**.

---

## Estrutura do Projeto

```text
├── assets/media/authors/me.png   # Foto de perfil
├── config/_default/              # Configurações do Hugo, idiomas, menus e tema
├── content/
│   ├── en/                       # Páginas e projetos em Inglês
│   └── pt/                       # Páginas e projetos em Português
├── data/
│   ├── authors/me.yaml           # Perfil, experiências e formação (EN)
│   └── pt/authors/me.yaml        # Tradução do perfil (PT-BR)
├── layouts/                      # Customizações locais de blocos
└── static/uploads/resume.pdf     # Currículo em PDF
```

---

## Como Executar Localmente

### Pré-requisitos

- [Hugo Extended](https://gohugo.io/installation/)
- [Node.js](https://nodejs.org/) e [pnpm](https://pnpm.io/)

### Comandos

```bash
# Instalar dependências
pnpm install

# Iniciar servidor local de desenvolvimento
pnpm run dev

# Gerar build de produção e índice de busca (Pagefind)
pnpm run build
```

---

## Contato

- **E-mail:** [marcosb@usp.br](mailto:marcosb@usp.br)

---

Baseado no template open-source [Hugo Blox Dev Portfolio](https://github.com/HugoBlox/kit) (licença MIT).
