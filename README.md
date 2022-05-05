# github-actions-ci-cd

### [.github/workflows/ci.yml](.github/workflows/ci.yml)

Essa action é responsável por executar todos os testes sempre que novos commits são enviados em qualquer branch (menos a `main`) e em em pull requests.

### [.github/workflows/cd.yml](.github/workflows/cd.yml)

Quando novos commits são enviados para a branch `main`, essa action:
  - Reusa a outra action [ci.yml](.github/workflows/ci.yml) para executar todos os testes.
  - Faz um novo deploy do app **se todos os testes passarem**.

## Learn more

- https://docs.github.com/en/actions/using-workflows/reusing-workflows
- https://docs.github.com/en/actions/using-workflows/triggering-a-workflow
