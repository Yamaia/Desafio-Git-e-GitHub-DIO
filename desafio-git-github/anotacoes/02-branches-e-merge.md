# Branches e merge

Uma **branch** é uma linha independente de desenvolvimento. A principal costuma ser `main`.

```bash
git branch                    # lista as branches
git switch -c feature/nome    # cria e entra em uma nova branch
git switch main               # volta para a main
git merge feature/nome        # traz as mudanças da branch para a atual
git branch -d feature/nome    # apaga a branch já mesclada
```

## Fluxo recomendado
1. Criar uma branch a partir da `main`.
2. Fazer os commits na branch.
3. Enviar a branch ao GitHub (`git push -u origin feature/nome`).
4. Abrir um Pull Request e fazer o merge.
5. Atualizar a `main` local (`git pull`).

## Conflitos de merge
Acontecem quando duas branches alteram o mesmo trecho. O Git marca o arquivo com `<<<<<<<`, `=======` e `>>>>>>>`. Basta escolher o conteúdo final, salvar, rodar `git add` e finalizar com `git commit`.
