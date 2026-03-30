# Relatório de Prontidão Técnica: Onboarding SecOps

**Disciplina:** Engenharia de Produto de Software (FGA0316) - 2026.1
**Aluno:** Lucas Soares Barros | **Matrícula:** 202017700

## 1. Configuração do Ambiente (Zero Trust & Isolamento)

Conforme as diretrizes de Soberania Técnica, as seguintes configurações foram aplicadas:

- [x] **Python 3.12:** Instalado e verificado.
- [x] **Poetry:** Configurado para criar `.venv` dentro do projeto (`virtualenvs.in-project true`).
- [x] **Determinismo:** Arquivos `pyproject.toml` e `poetry.lock` gerados com sucesso.

## 2. Logs de Auditoria e Qualidade (Security Gate)

Abaixo constam os resumos das execuções dos comandos de segurança:

### 2.1. Auditoria Estática (Bandit)

> Nenhuma vulnerabilidade encontrada.
> _Comando: `poetry run bandit -r core`_

### 2.2. Verificação de Dependências (Safety)

> Nenhuma vulnerabilidade encontrada nas dependências.
> _Comando: `poetry run safety check`_

### 2.3. Qualidade e Conformidade (Ruff)

> Nenhum problema de linter ou formatação encontrado após correções.
> _Comando: `poetry run ruff check . --fix && poetry run ruff format .`_

## 3. Evidência de Integração Contínua (CI)

O pipeline automatizado foi executado com sucesso no GitHub Actions:

- **Link da Action de Sucesso:** [https://github.com/lucaaassb/desafioSecOps/actions](https://github.com/lucaaassb/desafioSecOps/actions)

![CI](prints/Captura%20de%20tela%20de%202026-03-30%2017-42-52.png)

## 4. Declaração de Soberania Técnica (CISSP Domain 8)

Eu, Lucas Soares Barros, declaro que auditei manualmente as ferramentas e dependências deste projeto. Confirmo que o código gerado via IA (GitHub Copilot) passou pela minha revisão humana (_Human-in-the-loop_), garantindo que não há vazamento de segredos ou falhas lógicas críticas antes da migração para o ecossistema da PCDF.

---

**Data de Entrega:** 02/04/2026

## Observações Gerais e Específicas

- O projeto foi configurado seguindo as melhores práticas de SecOps, utilizando ferramentas para análise estática de segurança, verificação de dependências e qualidade de código.
- A integração contínua foi configurada para automatizar essas verificações a cada novo commit, garantindo que a base de código se mantenha segura e com qualidade.
- Os prints na pasta `prints` evidenciam a configuração do ambiente com Poetry, a execução do Bandit e o pipeline de CI em funcionamento.

![Poetry](prints/Captura%20de%20tela%20de%202026-03-30%2017-39-15.png)
![Bandit](prints/Captura%20de%20tela%20de%202026-03-30%2017-41-57.png)
