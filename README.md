# copsoq_indicadores
Validação Estrutural de Indicadores Psicossociais (ISP, IAT e NSP) via COPSOQ
Este repositório contém o código-fonte, dados simulados e especificações metodológicas para a validação da estrutura fatorial dos indicadores propostos no artigo: "Monitoramento de riscos psicossociais no trabalho: proposta de indicadores integrados a partir do COPSOQ versão portuguesa".

Informações do Repositório

Versão: v1.0.0 (Submission Release)
Data: Janeiro de 2026
Licença: MIT License
Idioma Principal: Português (Brasil)

Objetivo
Este projeto realiza uma Prova de Conceito (PoC) para validar a coerência estrutural dos indicadores:
ISP (Índice de Sobrecarga Psicológica)
IAT (Índice de Apoio no Trabalho)
NSP (Nível de Satisfação Psicológica)
A validação foi conduzida através de simulação computacional de dados (Monte Carlo) para testar a robustez estatística do modelo antes da aplicação empírica em larga escala.

Especificações Técnicas e Reprodutibilidade
Para garantir a reprodutibilidade total dos resultados apresentados no artigo, foram utilizados os seguintes parâmetros:
Semente Aleatória (Seed): 42
Tamanho da Amostra Simulada: N = 500
Método de Extração: Fatores Principais (Principal Axis Factoring - PAF)
Rotação: Varimax (Ortogonal)
Linguagem: Python 3.12+

Bibliotecas e Versões
As versões exatas das bibliotecas utilizadas estão listadas no arquivo requirements.txt.
pandas: 2.2.0
numpy: 1.26.0
factor-analyzer: 0.5.0

Estrutura de Arquivos
analise_validacao_copsoq.ipynb: Notebook do Google Colab com o código completo.
base_simulada_500_respostas.csv: O "Toy Dataset" gerado para o teste.
matriz_teorica_geradora.csv: Matriz de correlação teórica utilizada na simulação.
mapeamento_itens_indicadores.csv: Arquivo de referência que associa as perguntas do COPSOQ aos indicadores.
requirements.txt: Lista de dependências para instalação.

Como Executar
Clone este repositório:

Bash
git clone https://github.com/SEU_USUARIO/SEU_REPO.git
Instale as dependências:

Bash
pip install -r requirements.txt
Execute o notebook no ambiente de sua preferência (Jupyter ou Google Colab).

Citação
Se você utilizar este modelo ou código em sua pesquisa, por favor, cite:
[Igor Leo Rocha / IFBA]. (2026). Validação de Indicadores Psicossociais via Simulação. GitHub: https://www.youtube.com/watch?v=BW1w0P1KNk0.
