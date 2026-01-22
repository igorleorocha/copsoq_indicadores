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

analise_validacao_copsoq.ipynb: Código-fonte completo em Python (Jupyter Notebook/Google Colab). Contém todas as etapas de simulação, análise de fatores principais (PAF) com rotação Promax e cálculos de consistência interna.

base_simulada_500_respostas.csv: Contém 500 observações (linhas) e 41 colunas representando os itens do COPSOQ. Os dados seguem uma escala Likert de 1 a 5, gerados via simulação de Monte Carlo com a semente fixa (Seed 42).

cargas_fatoriais_promax.csv: Matriz de configuração (Pattern Matrix) que apresenta a carga de cada item do COPSOQ em seu respectivo indicador. Utilizada para confirmar a validade convergente e discriminante da estrutura proposta.

mapeamento_itens_indicadores.csv: Este arquivo atua como o dicionário de dados de referência do projeto. Ele correlaciona os itens do instrumento original COPSOQ-BR aos três indicadores propostos neste estudo (ISP, IAT e NSP).

matriz_correlacao_fatores.csv: Matriz de correlação interfatorial resultante da rotação oblíqua (Promax). Este arquivo apresenta os coeficientes de correlação entre os indicadores ISP, IAT e NSP, demonstrando a interdependência teórica e estatística dos construtos.

matriz_teorica_geradora.csv: Este arquivo contém a matriz de covariância/correlação definida a priori para a simulação de Monte Carlo. Ela detalha as correlações teóricas impostas entre os fatores latentes (ISP, IAT e NSP) antes da adição de ruído e erro de medição. 
mapeamento_itens_indicadores.csv: Dicionário de referência que correlaciona o número da questão no instrumento COPSOQ, o texto da pergunta e o indicador (ISP, IAT ou NSP) ao qual ela foi atribuída.

requirements.txt: Lista de dependências para instalação.

Como Executar

Clone este repositório:

Bash
git clone https://github.com/igorleorocha/copsoq_indicadores.git

Instale as dependências:

Bash
pip install -r requirements.txt

Execute o notebook no ambiente de sua preferência (Jupyter ou Google Colab).

Citação
Se você utilizar este modelo ou código em sua pesquisa, por favor, cite:
[Igor Leo Rocha / IFBA]. (2026). Validação de Indicadores Psicossociais via Simulação. GitHub: https://www.youtube.com/watch?v=BW1w0P1KNk0.
