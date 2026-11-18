# Entregável 7 – Entrega Parcial do Projeto Final (Semana 14)

Estrutura escalável do Projeto Final em React organizada em `components`, `pages`, `services`, `contexts` e `hooks`, com React Router, Tailwind CSS e `ThemeContext` persistido no `localStorage`.

## Parte 4 – Reflexão (Para Pensar)

**Qual a importância de separar as páginas (`pages`) dos componentes reutilizáveis (`components`) e da lógica de API (`services`) em um projeto React que está crescendo?**

- **Separação de responsabilidades (Clean Architecture):**
  - **`components/`:** Guarda peças visuais puras e reutilizáveis (`Button`, `Card`, `Header`) que podem ser usadas em qualquer tela sem duplicar código.
  - **`pages/`:** Representa cada rota/tela da aplicação (`Home`, `Catalogo`, `Sobre`), orquestrando quais componentes e dados aparecem em cada URL.
  - **`services/`:** Isola as chamadas `fetch` e URLs de API em um único lugar. Se o endereço da API mudar no futuro, alteramos apenas o arquivo `services/api.js` em vez de procurar chamadas espalhadas por dezenas de componentes, facilitando testes e manutenção em equipe.
