# quizzes-martina

Quizzes de estudo da Martina (3º ano), publicados automaticamente no Vercel a cada push na branch `main`.

## Estrutura
- `index.html` — Mural de Missões (página inicial com todos os quizzes).
- `<tema-slug>/index.html` — um quiz por pasta. Link: `https://<projeto>.vercel.app/<tema-slug>/`

## Como adicionar um quiz
1. Criar a pasta `<tema-slug>/` com o `index.html` do quiz (arquivo único, sem dependências).
2. Adicionar a missão no array `missoes` do `index.html` da raiz (mais recente primeiro).
3. Commit + push na `main` → o Vercel publica sozinho.
