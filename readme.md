# Publicar o curriculo com GitHub Actions + GitHub Pages

## 1. Subir o projeto no GitHub

No terminal, dentro da pasta do projeto:

git init
git add .
git commit -m "feat: curriculo inicial"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/NOME-DO-REPO.git
git push -u origin main

## 2. Workflow de deploy

Este projeto ja tem o workflow em [.github/workflows/deploy-pages.yml](.github/workflows/deploy-pages.yml).

Ele faz deploy automatico no GitHub Pages quando houver push na branch main.

## 3. Ativar o GitHub Pages

No repositorio no GitHub:

1. Abra Settings
2. Abra Pages
3. Em Build and deployment, escolha Source: GitHub Actions

## 4. Encontrar o link publico

Depois que o workflow terminar com sucesso, o site fica em:

https://SEU-USUARIO.github.io/NOME-DO-REPO/

Se o repositorio se chamar SEU-USUARIO.github.io, o link vira:

https://SEU-USUARIO.github.io/

## 5. Como atualizar o site

Sempre que editar os arquivos e fizer push na main, o GitHub Actions publica a nova versao automaticamente.

