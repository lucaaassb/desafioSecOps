# 🚀 Desafio 01 — Onboarding SecOps & Soberania Técnica

## 📌 Objetivo

Este projeto tem como objetivo demonstrar a configuração de um ambiente seguro e padronizado seguindo práticas de **DevSecOps**, conforme os princípios do Domínio 8 do CISSP (Software Development Security).

A proposta garante que a segurança seja aplicada desde o início do ciclo de desenvolvimento (Shift Left), utilizando auditoria contínua e validações automatizadas.

---

## 🧱 Stack Utilizada

* Python 3.12
* Django
* Poetry (gerenciamento de dependências)
* Docker
* Bandit (SAST)
* Safety (SCA)
* Ruff (Linter/Formatter)
* GitHub Actions (CI/CD)

---

## ⚙️ Evidência de Ambiente

Ambiente configurado com **Python 3.12** utilizando Poetry, garantindo isolamento através de virtual environment local.

📸 **Evidência:**
![Ambiente Poetry](./prints/poetry-env.png)

---

## 🔐 Segurança da Aplicação

### ✔️ SAST — Bandit

Foi realizada análise estática de segurança no código utilizando Bandit.

* Identificação de vulnerabilidades
* Remoção de segredo hardcoded (SECRET_KEY)
* Aplicação de boas práticas de segurança

📸 **Evidência:**
![Bandit Scan](./prints/bandit.png)

---

### ✔️ SCA — Safety

Validação de vulnerabilidades em bibliotecas de terceiros, garantindo integridade das dependências.

---

### ✔️ Linter — Ruff

Padronização e qualidade do código seguindo boas práticas de desenvolvimento Python.

---

## 🐳 Containerização com Docker

A aplicação foi isolada utilizando Docker, garantindo:

* Ambiente reproduzível
* Isolamento de execução
* Preparação para ambientes controlados (on-premise)

---

## ⚙️ Integração Contínua (CI)

Pipeline configurado no GitHub Actions executando:

* Bandit (SAST)
* Ruff (Lint)
* Safety (SCA)

📸 **Evidência do Pipeline:**
![CI Passing](./prints/ci.)

---

## 🛡️ Práticas de Segurança Aplicadas

* Remoção de segredo hardcoded (SECRET_KEY)
* Uso de variáveis de ambiente (.env)
* Exclusão de arquivos sensíveis via `.gitignore`
* Validação contínua via pipeline CI
* Auditoria automatizada (SAST + SCA)

---

## ✅ Declaração de Prontidão

O ambiente foi configurado com sucesso, atendendo aos requisitos de:

* Segurança (SAST e SCA aprovados)
* Qualidade de código (Lint aprovado)
* Pipeline de CI funcional (Build Passing)
* Isolamento via Docker

O projeto está pronto para integração em ambiente organizacional seguindo práticas de **DevSecOps** e **Soberania Técnica**.

---

## 📅 Status

✔️ Ambiente configurado
✔️ Segurança validada
✔️ CI/CD funcionando
✔️ Pronto para migração

---

## 📁 Observação

Criar uma pasta chamada `prints` na raiz do projeto e adicionar:

* `poetry-env.png`
* `bandit.png`
* `ci.png`

---
