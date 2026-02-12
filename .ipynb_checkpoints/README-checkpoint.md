{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "7aa3725b-a981-4176-b1dc-f9d18b7544a9",
   "metadata": {},
   "source": [
    "# 📊 Desafio Técnico — Estágio em Desenvolvimento de Dados  \n",
    "Fato Analytics\n",
    "\n",
    "Este repositório contém a solução desenvolvida para o desafio técnico do processo seletivo.\n",
    "\n",
    "O objetivo foi transformar dados brutos de um CRM (planilha Excel) em indicadores estruturados e insights relevantes para o negócio.\n",
    "\n",
    "---\n",
    "\n",
    "## 🧱 Estrutura do Projeto\n",
    "\n",
    "- `01_certificacao_dados.ipynb` → Tratamento e validação dos dados  \n",
    "- `02_camada_analitica.ipynb` → Construção dos indicadores  \n",
    "- `dados_tratados.db` → Banco SQLite com dados certificados  \n",
    "- `relatorio_executivo.md` → Explicação completa da estratégia e análises  \n",
    "\n",
    "Após a etapa de tratamento, o Excel deixa de ser utilizado.  \n",
    "O SQLite passa a ser a fonte oficial do projeto.\n",
    "\n",
    "---\n",
    "\n",
    "## 📈 Dashboard Executivo\n",
    "\n",
    "O painel foi construído no Metabase, conectado diretamente ao banco SQLite.\n",
    "\n",
    "Principais análises apresentadas:\n",
    "\n",
    "- Receita total e mensal  \n",
    "- Lucro total  \n",
    "- Margem média  \n",
    "- Meta vs realizado (mensal)  \n",
    "- Receita por canal  \n",
    "- Concentração por produto  \n",
    "\n",
    "### 📷 Visual do Dashboard\n",
    "\n",
    "![Dashboard Executivo](dashboard/dashboard.png)\n",
    "\n",
    "---\n",
    "\n",
    "## 🚀 Execução\n",
    "\n",
    "Pré-requisitos:\n",
    "- Python 3.9+\n",
    "- Jupyter Notebook\n",
    "- pandas\n",
    "\n",
    "1. Executar `01_certificacao_dados.ipynb` → Gera o banco `dados_tratados.db`\n",
    "2. Executar `02_camada_analitica.ipynb` → Constrói as tabelas analíticas\n",
    "3. Conectar o Metabase ao arquivo `dados_tratados.db` → Criar dashboard utilizando as tabelas analíticas\n",
    "\n",
    "---\n",
    "\n",
    "## 📄 Observação\n",
    "\n",
    "A documentação completa da estratégia, decisões técnicas e análise de resultados está disponível em `relatorio_executivo.ipynb`."
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.8.10"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
