# 🛠️ Log de Desenvolvimento

Aqui está um registro cronológico do que ocorreu durante a nossa sessão:

## 1. Do Link-in-Bio para Landing Page
A estrutura inicial tinha um CSS embutido usando TailwindCSS através do CDN. Nós estruturamos um plano de ação (presente no artefato de *implementation_plan*) para criar seções de:
- Hero Section
- Coleção e Destaques
- Sobre Nós
- Benefícios
- Contato

## 2. Refinamento de Escopo
Após entregar a página completa, recebemos o pedido para **remover** as seções de Coleção, Sobre a Marca e Benefícios, mantendo a página o mais objetiva e limpa possível.
> **Ação realizada:** O arquivo `code.html` foi editado para remover essas seções e limpar as âncoras (`#colecao`, `#sobre`) dos menus.

## 3. Configuração do Servidor Local (Vite)
Para facilitar o desenvolvimento, rodamos o comando para instalar o servidor local.
- **Problema:** Apenas rodar `code.html` no navegador estático não fornece "Hot Reload".
- **Solução:** Criamos um arquivo `package.json` para adicionar a dependência do `vite` (`npm install -D vite`) e configuramos o script `"dev": "vite"`.

## 4. O Desafio Mobile e o Firewall do Windows
O objetivo era ver a página sendo executada direto no smartphone usando a rede Wi-Fi.
- **Passo 1:** Adicionamos a flag `--host` no `package.json` para expor o localhost para a rede (IP do tipo 192.168.x.x).
- **Passo 2:** O arquivo chamava-se `code.html`, obrigando o usuário a digitar o link completo na URL (`/code.html`). Renomeamos o arquivo para `index.html`, pois o Vite o serve por padrão como página principal.
- **Passo 3:** Identificamos que quando nada carrega (fica apenas a tela de *loading* eterna no celular), costuma ser culpa do Firewall do Windows bloqueando portas (neste caso, a 5173). Nós até tentamos rodar o comando PowerShell `New-NetFirewallRule` remotamente, mas houve "Acesso Negado" por falta de privilégios de Administrador. A solução repassada foi confirmar o aviso de permissão que o Windows exibe ou mudar a rede de Pública para Privada.

## 5. Integração com Obsidian
E finalmente, atendemos ao pedido de transformar toda essa experiência e conhecimento em uma base de dados pro Obsidian! Tudo interligado, com arquivos `.md` e imagens armazenadas localmente.
