# OWS Documentation Hub

Bem-vindo ao repositório central de documentação do time OWS.

Esta documentação utiliza GitHub Pages e a ferramenta [MkDocs](https://www.mkdocs.org/) com o tema builtin ReadTheDocs.

A [página web da documentação](https://symmetrical-doodle-e4qkelp.pages.github.io/) é privada e acessível apenas para quem tem acesso a este repositório GitHub.

## Estrutura do repositório

```
/README.md           -> Este documento
/mkdocs/             -> Local para edição da documentação e configuração do mkdocs
/mkdocs/mkdocs.yml   -> Arquivo de configuração do mkdocs
/mkdocs/docs/        -> Arquivos fonte da documentação em Markdown
```

## Como usar

### Pré-requisitos

- Python 3.9+
- MkDocs instalado (`pip install mkdocs`)

### Adicionando uma nova página

1. Crie um arquivo `.md` dentro de `mkdocs/docs/`:
   ```bash
   touch mkdocs/docs/minha-pagina.md
   ```

2. Edite o arquivo com o conteúdo desejado usando Markdown.

3. Adicione a página na navegação editando `mkdocs/mkdocs.yml`:
   ```yaml
   nav:
     - Home: index.md
     - Minha Página: minha-pagina.md
   ```

4. (Opcional) Visualize localmente antes de fazer push:
   ```bash
   cd mkdocs
   mkdocs serve
   ```
   Acesse `http://127.0.0.1:8000` no navegador.

5. Faça commit e push para a branch `main`. A pipeline irá gerar e publicar o site automaticamente via GitHub Pages.

### Referências

- [Getting Started with MkDocs](https://www.mkdocs.org/getting-started/)
- [MkDocs - Writing your docs](https://www.mkdocs.org/user-guide/writing-your-docs/)

## Manutenção

Este repositório é mantido pela equipe OWS. Para sugestões ou dúvidas, abra uma issue.
