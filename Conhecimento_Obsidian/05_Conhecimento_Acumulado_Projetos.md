# 🧠 Conhecimento Acumulado (Todos os Projetos)

Este documento centraliza todo o conhecimento adquirido, soluções de problemas e padrões de design estabelecidos em nossas interações e projetos passados, atendendo ao pedido de consolidação total de aprendizados.

## 1. Design System e Identidade (Velvet & Rose)
Foi definido um padrão rigoroso de UI/UX chamado "Chic Editorial" para landing pages de alta conversão na moda feminina.
- **Cores Principais:** Superfície clara (`#f7f9ff` e `#ffffff`), detalhes em Rosa Chiclete/Vinho (`#b5106a`), contrastando com textos escuros (`#181c20`).
- **Tipografia:** 
  - *Bodoni Moda* (Serifada) para títulos e logos, passando alto impacto e luxo.
  - *Hanken Grotesk* (Sem-Serifa) para textos corridos, links e botões, focando em legibilidade mobile.
- **Micro-interações:** Uso de "Glassmorphism" (Efeito de vidro fosco) em barras de navegação fixas para manter leveza visual. Sombras sempre tonais (tintadas com a cor primária, não apenas cinza) para dar profundidade natural.

## 2. Soluções de UI/UX e Animações Desenvolvidas
- **Animações Sincronizadas (Efeito Flash & Elasticidade):** Desenvolvemos um efeito visual onde um "flash" de luz passa sobre um elemento. Sincronizado a esse flash, criamos uma animação onde *cada letra do texto* balança individualmente para a direita e volta para a posição (efeito elástico leve), sem mover o bloco inteiro do texto.
- **Curvatura de Texto Customizada:** Textos foram adaptados via CSS/SVG para seguirem curvaturas idênticas a logotipos específicos (como a curvatura do texto "Chique").
- **Responsividade Fluida de Componentes:** Definimos regras flexíveis de CSS (usando rem, porcentagens e media queries) para garantir que não apenas textos, mas todos os **botões se ajustem dinamicamente** ao tamanho exato da tela de qualquer smartphone.

## 3. Infraestrutura, Configurações e Deploy
- **Tag Title:** O conhecimento sobre como alterar o nome que é exibido na aba do navegador (removendo o "link do deploy"). Isso é feito diretamente através da tag `<title>Nome Desejado</title>` dentro da seção `<head>` do arquivo `index.html`.
- **Controle de Versão (GitHub):** Estabelecemos a prática contínua de salvar e versionar os arquivos no GitHub, garantindo backup do repositório para facilitar atualizações em serviços de Deploy.
- **Servidor de Teste Local (Vite):** 
  - Instalamos o Vite para garantir *Hot Reload* nas edições.
  - Acessamos o servidor pelo smartphone na mesma rede local usando o comando com flag de rede (`npm run dev -- --host`).
  - Identificamos e lidamos com bloqueios do **Firewall do Windows** que impediam a porta 5173 de ser acessada por dispositivos externos.
- **Limpeza de Escopo (Foco em Conversão):** Aprendizado prático de que uma página estilo "Link-in-bio" funciona melhor sendo direta e agressiva para a conversão. Seções como "Sobre a Marca" e "Coleções extras" foram descartadas do HTML para focar o usuário no botão principal.
