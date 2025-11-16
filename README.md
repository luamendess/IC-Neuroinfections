Este espaço será dedicado ao desenvolvimento da minha Iniciação Científica

> Projeto: Exploração de assinaturas de expressão gênica humana para melhorar a sensibilidade de testes metagenômicos no diagnóstico de neuroinfecções.

> Obejtivo: propor uma abordagem integrada, baseada em dados públicos, que combina mNGS e análise da expressão gênica humana para aprimorar o diagnóstico da meningite tuberculosa - por meio da identificação e avaliação de assinaturas de expressão gênica capazes de discriminar casos de tuberculose meníngea, utilizando pipelines reprodutíveis e técnicas de aprendizado de máquina conforme a metodologia descrita na literatura. 

---

# Pipeline de Análise – Neuroinfections IC

Este repositório contém o ambiente, organização e pipeline inicial para desenvolvimento da Iniciação Científica relacionada ao projeto **Neuroinfections**.
Aqui estão descritas as etapas de instalação, configuração do ambiente, estrutura do projeto e fluxos de trabalho básicos utilizados ao longo da pesquisa.

---

## 1. Estrutura do Projeto

```
Neuroinfections/
│── data/                       # Dados brutos e processados
│── notebooks/                  # Notebooks adicionais
│── src/                        # Scripts auxiliares da pipeline
│── pipeline.ipynb              # Pipeline principal de análise
│── README.md                   # Documentação do projeto
│── .gitignore                  # Arquivos ignorados pelo Git
│── .venv/                      # Ambiente virtual (ignorado pelo Git)
```

---

## 2. Ambiente Virtual (venv)

Este projeto utiliza um ambiente virtual isolado para garantir reprodutibilidade e controle das dependências.

### Criar o ambiente virtual

```
python -m venv .venv
```

### Ativar o ambiente virtual (Git Bash)

```
source .venv/Scripts/activate
```

### Instalar as dependências dentro da venv

```
pip install jupyter pandas numpy matplotlib seaborn scikit-learn
```

---

## 3. Jupyter Notebook

Após ativar a venv, abra o `pipeline.ipynb` no VS Code e selecione o kernel correspondente ao ambiente virtual:

```
Python 3.x (.venv)
```

Caso necessário, selecione manualmente o interpretador:

```
Neuroinfections/.venv/Scripts/python.exe
```

---

## 4. Arquivo .gitignore

Para evitar que arquivos desnecessários sejam enviados ao repositório:

```
.venv/
__pycache__/
.ipynb_checkpoints/
```

---

## 5. Fluxo Básico de Git

### Adicionar arquivos ao commit

```
git add .
```

### Criar commits

```
git commit -m "mensagem do commit"
```

### Associar o repositório remoto (primeira vez)

```
git remote add origin https://github.com/luamendess/IC-Neuroinfections
git branch -M main
git push -u origin main
```

### Enviar alterações para o GitHub

```
git push
```

### Obter alterações do repositório remoto

```
git pull origin main
```

### Resolver conflitos

Arquivos com conflito apresentam marcações como:

```
<<<<<<< HEAD
(seu código)
=======
(código remoto)
>>>>>>> origin/main
```

Ajuste o conteúdo final, depois:

```
git add arquivo
git commit -m "resolve conflito"
git push
```

---

## 6. Limpeza e Otimização do Repositório

```
git gc --prune=now
git prune
```

---

## 7. Estrutura da Pipeline no Notebook

```
- Controle de Qualidade das sequências
- Remoção de contaminantes
- Taxonimia
- Montagem De novo
- Anotação e validação 
- Laudo
```

## 8. Objetivo do Repositório

Este repositório tem como objetivo organizar e documentar toda a pipeline analítica utilizada na Iniciação Científica do projeto **Neuroinfections**, garantindo controle de versão, padronização e reprodutibilidade.

---