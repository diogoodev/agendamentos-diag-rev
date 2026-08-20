# 🔧 Rodízio de Agendamento da Oficina

Sistema web para gerenciar e automatizar a escala de atendimentos de uma oficina mecânica, garantindo um rodízio justo e equilibrado entre os mecânicos.

## ✨ Funcionalidades

- **Atribuição automática com 1 clique** — distribui Diagnósticos e Revisões ao mecânico com menor carga
- **Algoritmo de equilíbrio** — prioriza quem tem menos atendimentos do tipo solicitado; em caso de empate, usa FIFO
- **Histórico de agendamentos** — registro dos últimos atendimentos com horário e identificação da O.S.
- **Persistência local** — dados salvos via `localStorage`, sem necessidade de servidor ou banco de dados
- **Zero dependências** — HTML + CSS + JS puro, funciona em qualquer navegador

## 👨‍🔧 Equipe

| Mecânico      |
|---------------|
| Orlando       |
| Francisco     |
| Cristiano     |
| Sandro        |
| Joao Carlos   |
| Tassio        |

## 🚀 Como usar

### Online
Acesse diretamente pelo link da Vercel (ver seção de deploy abaixo).

### Localmente
Basta abrir o arquivo `index.html` diretamente no navegador — não precisa de servidor web.

## 🛠️ Tech Stack

- **HTML5** — estrutura
- **CSS3** — estilização (tema escuro, responsivo)
- **JavaScript (ES6+)** — lógica de negócio e persistência via `localStorage`
- **Single File App** — tudo em um único `index.html`

## 📋 Regras de Negócio

1. Ao clicar em **Atribuir Diagnóstico** ou **Atribuir Revisão**, o sistema seleciona automaticamente o mecânico com menor contagem daquele tipo de serviço.
2. Em caso de empate na contagem, prioriza quem foi escalado há mais tempo (FIFO por timestamp).
3. O botão **Zerar Contagens** reseta todo o histórico (com confirmação).
4. Todos os dados ficam salvos no navegador via `localStorage`.

## 📦 Deploy

### GitHub Pages
O site é publicado automaticamente via GitHub Pages na branch `main`.

### Vercel
Deploy automático conectado ao repositório GitHub — qualquer push na `main` atualiza o site em produção.

---

Desenvolvido para uso interno da oficina. 🔩
