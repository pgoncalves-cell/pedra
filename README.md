# Pedra — Site institucional

Landing page estática (HTML + CSS puro) da Pedra, com soluções em **Mineração**, **Concreto** e **Pavimentação**.

## Estrutura

```
.
├── index.html       # página principal
├── style.css        # estilos base (Tailwind compilado)
├── custom.css       # pequenos ajustes (grid de 3 colunas, fonte)
└── logo-pedra.png   # logotipo
```

Todos os arquivos ficam na mesma pasta, sem subdiretórios — só copiar tudo e subir para o repositório.

## Rodar localmente

Não precisa de build nem dependências. Basta abrir `index.html` no navegador, ou servir a pasta com qualquer servidor estático, por exemplo:

```bash
python3 -m http.server 8000
```

e acessar `http://localhost:8000`.

## Publicar no GitHub Pages

1. Crie um repositório no GitHub e suba estes arquivos (`git init`, `git add .`, `git commit`, `git push`).
2. No repositório, vá em **Settings → Pages**.
3. Em "Source", selecione a branch `main` e a pasta `/ (root)`.
4. Salve. O site ficará disponível em `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`.

## Personalização

- Textos e seções: editar diretamente `index.html`.
- Cores, espaçamentos e componentes customizados: `custom.css`.
- Formulário de contato: envia via `mailto:`, abrindo o app de e-mail do visitante. Para receber submissões diretamente (sem abrir o e-mail do usuário), será necessário integrar um serviço de formulário (ex: Formspree, Getform) ou um backend próprio.
