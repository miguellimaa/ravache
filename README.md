# Atividade Node.js + Docker + GitHub Actions

Este repositorio preserva a aplicacao Hello World da atividade anterior. O arquivo original se chama `node index.js` (com espaco no nome).

## Executar com Node.js

Requisito: Node.js 20 ou superior.

```bash
npm start
```

Acesse http://localhost:3000 para visualizar **Hello World!**.

## Executar com Docker

```bash
docker build -t ravache-node .
docker run --rm -p 3000:3000 ravache-node
```

Acesse http://localhost:3000.

## GitHub Actions

O workflow em `.github/workflows/ci.yml` e acionado em push e pull request. Ele verifica a sintaxe do arquivo JavaScript, constroi a imagem Docker, inicia o container e testa se a rota inicial retorna `Hello World!`.

O resultado pode ser acompanhado na aba **Actions** do repositorio.
