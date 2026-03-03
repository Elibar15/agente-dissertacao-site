# Publicar site grátis (GitHub Pages)

## 1) Criar repositório no GitHub
1. Ir a https://github.com/new
2. Nome sugerido: `agente-dissertacao-site`
3. Criar como público (ou privado com Pages disponível no teu plano)

## 2) Enviar esta pasta `site`
No terminal, dentro da pasta do projeto:

```bash
cd "Agente de Apoio Dissertação/site"
git init
git add .
git commit -m "Site base para agente de apoio a dissertacao"
git branch -M main
git remote add origin https://github.com/SEU_UTILIZADOR/agente-dissertacao-site.git
git push -u origin main
```

## 3) Ativar GitHub Pages
1. No repositório, abrir `Settings` > `Pages`
2. Em `Build and deployment`, escolher:
   - `Source`: Deploy from a branch
   - `Branch`: `main` e pasta `/ (root)`
3. Guardar

URL final típica:
`https://SEU_UTILIZADOR.github.io/agente-dissertacao-site/`

## 4) Ligar ao Agent Builder
1. Abrir Agent Builder
2. `Knowledge` > `Add specific websites`
3. Adicionar:
   - URL inicial: `https://SEU_UTILIZADOR.github.io/agente-dissertacao-site/`
   - e cada página específica (registo, submissão, FAQ, etc.)
4. Ativar `Only use specified sources`

## 5) Atualizar conteúdo
Sempre que alterares texto:

```bash
git add .
git commit -m "Atualiza conteudo oficial"
git push
```

O site costuma atualizar em 1-3 minutos.
