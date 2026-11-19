---
title: ''
summary: ''
date: 2026-11-19
type: landing

sections:
  # Developer Hero
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "Olá, eu sou"
      show_status: true
      show_scroll_indicator: true
      typewriter:
        enable: true
        prefix: "Eu desenvolvo"
        strings:
          - "apps mobile em React Native"
          - "integrações BLE com hardware"
          - "aplicações desktop em Tauri & Rust"
          - "interfaces web modernas"
        type_speed: 70
        delete_speed: 40
        pause_time: 2500
      cta_buttons:
        - text: Ver Projetos
          url: "#projects"
          icon: arrow-down
        - text: Entrar em Contato
          url: "#contact"
          icon: envelope
    design:
      style: centered
      avatar_shape: circle
      animations: true
      background:
        color:
          light: "#fafafa"
          dark: "#0a0a0f"
      spacing:
        padding: ["6rem", "0", "4rem", "0"]

  # Filterable Portfolio
  - block: portfolio
    id: projects
    content:
      title: "Projetos em Destaque"
      subtitle: "Aplicativos mobile, telemetria via BLE e design de interfaces"
      count: 0
      filters:
        folders:
          - projects
      buttons:
        - name: Todos
          tag: '*'
        - name: Mobile
          tag: Mobile
        - name: BLE & IoT
          tag: BLE & IoT
        - name: Design UI/UX
          tag: Design UI/UX
      default_button_index: 0
    design:
      columns: 2
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Visual Tech Stack
  - block: tech-stack
    id: skills
    content:
      title: "Tecnologias & Ferramentas"
      subtitle: "Linguagens, frameworks, hardware e ferramentas do meu dia a dia"
      categories:
        - name: Linguagens
          items:
            - name: JavaScript
              icon: devicon/javascript
            - name: C
              icon: devicon/c
            - name: C++
              icon: devicon/cplusplus
            - name: Rust
              icon: devicon/rust
            - name: HTML5
              icon: devicon/html5
            - name: CSS3
              icon: devicon/css3
        - name: Mobile & Desktop
          items:
            - name: React Native
              icon: devicon/react
            - name: Tauri
              icon: devicon/tauri
            - name: Bluetooth LE
              icon: brands/bluetooth
        - name: Hardware & Engenharia
          items:
            - name: Arduino
              icon: devicon/arduino
            - name: NI LabView
              icon: devicon/labview
            - name: Multisim
              icon: hero/cpu-chip
        - name: Ferramentas & IA
          items:
            - name: Git
              icon: devicon/git
            - name: Figma
              icon: devicon/figma
            - name: Azure
              icon: devicon/azure
            - name: Notion
              icon: devicon/notion
            - name: Claude
              icon: brands/claude
            - name: OpenAI Codex
              icon: brands/openai
    design:
      style: grid
      show_levels: false
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Experience & Education Timeline (reads from data/pt/authors/me.yaml)
  - block: resume-experience
    id: experience
    content:
      username: me
    design:
      date_format: Jan 2006
      is_education_first: false
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Contact Section
  - block: contact-info
    id: contact
    content:
      title: Contato
      subtitle: "Vamos construir algo de impacto juntos"
      connect_title: "Vamos Conversar"
      text: |-
        Estudante de Engenharia Elétrica na USP interessado em inovação, engenharia de software e produtos conectados a hardware.
        Fique à vontade para entrar em contato!
      email: marcosb@usp.br
      autolink: true
    design:
      columns: '1'
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # CTA Card
  - block: cta-card
    content:
      title: "Baixar Currículo"
      text: |-
        Confira todos os detalhes da minha formação na **Poli-USP**, Iniciação Científica no **IPEN** e experiências no **BTG Pactual**, **ZYLA** e **Mercado Bitcoin**.
      button:
        text: 'Baixar CV (PDF)'
        url: uploads/resume.pdf
        new_tab: true
    design:
      card:
        css_class: 'bg-gradient-to-br from-primary-200 via-primary-100 to-secondary-200 dark:from-primary-600 dark:via-primary-700 dark:to-secondary-700'
        text_color: dark
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "6rem", "0"]
---
