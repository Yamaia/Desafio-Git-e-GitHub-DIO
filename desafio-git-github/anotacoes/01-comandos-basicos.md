# Comandos básicos do Git

## Configuração inicial
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

## Ciclo básico
```bash
git init                      # cria o repositório local
git status                    # vê o que mudou
git add arquivo.md            # adiciona um arquivo ao stage (ou: git add .)
git commit -m "docs: mensagem" # registra a versão
git log --oneline             # histórico resumido
git diff                      # mostra as diferenças ainda não commitadas
```

## Áreas do Git
1. **Working directory**: onde você edita os arquivos.
2. **Staging area**: onde ficam os arquivos prontos para o commit (`git add`).
3. **Repositório**: onde as versões ficam gravadas (`git commit`).

## Boas práticas de commit
- Mensagens curtas e no imperativo/descritivas: `docs: adiciona anotações de branches`.
- Um commit por mudança lógica.
- Prefixos comuns: `feat`, `fix`, `docs`, `refactor`, `chore`.

## .gitignore
Arquivo que lista o que o Git deve ignorar (ex.: `node_modules/`, `.env`, `__pycache__/`).
