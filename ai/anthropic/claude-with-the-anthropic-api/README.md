# claude-with-the-anthropic-api

Ambiente Python com Jupyter Notebook para explorar a API da Anthropic.

## Pré-requisitos

- [uv](https://astral.sh/uv) instalado
- VSCode com a extensão **Jupyter** (Microsoft)

## Setup

### 1. Criar o projeto

```bash
uv init claude-with-the-anthropic-api
cd claude-with-the-anthropic-api
```

### 2. Instalar dependências

```bash
uv add notebook ipykernel requests
```

### 3. Ativar o virtualenv

```bash
source .venv/bin/activate
```

### 4. Registrar o kernel no Jupyter

```bash
python -m ipykernel install --user --name=claude-with-the-anthropic-api
```

---

Pronto para rodar notebooks. 🚀

## Rodando um notebook

1. Abra o VSCode na pasta do projeto
2. Crie um arquivo `.ipynb` ou use `Ctrl+Shift+P` → `Create: New Jupyter Notebook`
3. No canto superior direito, clique em **Select Kernel** → escolha `claude-with-the-anthropic-api`
4. Comece a explorar

## Estrutura sugerida

```
claude-with-the-anthropic-api/
├── .venv/               # virtualenv (não sobe pro Git)
├── .gitignore
├── pyproject.toml       # dependências gerenciadas pelo uv
├── notebooks/
│   └── explorar.ipynb
└── README.md
```

## .gitignore

```
.venv/
__pycache__/
.ipynb_checkpoints/
```