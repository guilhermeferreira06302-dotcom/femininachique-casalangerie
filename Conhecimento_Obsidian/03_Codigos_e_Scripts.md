# 💻 Códigos e Scripts

Aqui estão guardadas as referências diretas de código geradas.

## `package.json`

O arquivo configurado para rodar a aplicação via Vite na rede local para testes mobile. A flag `--host` garante a exposição do IP e a flag `--open` abre no navegador automaticamente.

```json
{
  "name": "stitch-bio-links-moda-feminina",
  "version": "1.0.0",
  "description": "Landing page",
  "scripts": {
    "dev": "vite --host --open"
  },
  "devDependencies": {
    "vite": "^5.2.0"
  }
}
```

## `index.html` (Landing Page Principal)

Nota: Originalmente chamado de `code.html`, foi renomeado para facilitar a renderização pelo Vite sem a necessidade de passar caminhos complexos na URL.

*(A página utiliza Tailwind via CDN com configurações embutidas. Acesse o arquivo `index.html` na raiz do projeto original para inspecionar o código completo. Ele implementa propriedades de Glassmorphism, Fade-Ins e fontes externas importadas via Google Fonts: Hanken Grotesk e Bodoni Moda).*
