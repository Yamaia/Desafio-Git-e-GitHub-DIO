# GitHub e Pull Requests

## Sincronização com o repositório remoto
```bash
git remote add origin https://github.com/USUARIO/REPO.git
git push -u origin main     # primeiro envio
git push                    # envios seguintes
git pull                    # baixa e integra mudanças do remoto
git clone URL               # copia um repositório remoto
```

## Pull Request (PR)
Pedido para mesclar as mudanças de uma branch em outra. Serve para revisão de código, discussão e histórico.

### Passo a passo
1. Envie a branch com `git push -u origin nome-da-branch`.
2. No GitHub, clique em **Compare & pull request**.
3. Descreva o que mudou e por quê.
4. Faça o merge (**Merge pull request**).

## Fork
Cópia de um repositório de outra pessoa para a sua conta, usada para contribuir com projetos que você não tem permissão de escrita.

## README.md
É a "vitrine" do projeto: explica o que é, como usar e a estrutura. Escrito em Markdown.
