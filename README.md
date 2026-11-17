# quizzes-martina

Quizzes de estudo da Martina (3º ano), publicados automaticamente no Vercel a cada push na branch `main`.

## Estrutura
- `index.html` — Biblioteca da Martina (página inicial, agrupada por matéria, com botões "Ver resumo" e "Fazer o quiz").
- `<materia>/<tema-slug>/index.html` — o quiz.
- `<materia>/<tema-slug>/resumo.pdf` — o resumo em PDF (o botão só aparece quando o arquivo existe).
- Links antigos (`/<tema-slug>/`) redirecionam para o novo caminho via `vercel.json`.

## Como adicionar um estudo
1. Criar a pasta `<materia>/<tema-slug>/` com o `index.html` do quiz e o `resumo.pdf`.
2. Adicionar o estudo no array `estudos` do `index.html` da raiz (mais recente primeiro).
3. Commit + push na `main` → o Vercel publica sozinho.
