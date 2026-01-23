Framework de Indicadores de Riscos Psicossociais (COPSOQ-PT)

Este repositório contém os materiais, scripts e conjuntos de dados sintéticos referentes ao estudo metodológico de validação exploratória de indicadores psicossociais baseados na versão curta do Copenhagen Psychosocial Questionnaire (COPSOQ-PT).

Sobre o Projeto

O objetivo deste projeto é propor uma simplificação das dimensões multidimensionais do COPSOQ-PT em três indicadores sintéticos para fins de gestão de Saúde e Segurança do Trabalho (SST) e conformidade com a NR-1 e o eSocial:

- Índice de Sobrecarga Psicológica (ISP): Mede demandas quantitativas, cognitivas e emocionais.

-Índice de Apoio no Trabalho (IAT): Mede suporte social, liderança e justiça organizacional.

- Nível de Satisfação Psicológica (NSP): Mede autonomia, significado do trabalho e engajamento.

Metodologia e Simulação

Visto que este é um estudo exploratório preliminar, os dados foram gerados via Simulação de Monte Carlo (N=500), garantindo um ambiente controlado para o teste de estresse da plausibilidade estrutural do modelo.

Parâmetros da Simulação

Tamanho da Amostra: 500 observações.

Estrutura: 41 itens (conforme COPSOQ-PT versão curta).

Semente Aleatória: 42 (para reprodutibilidade).

Linguagem: Python 3.12.

Estrutura do Repositório

analise_fatorial_final.py: Script Python utilizado para simulação de dados e análise estatística.

dataset_simulado_41_itens.csv: Base de dados sintética bruta (respostas de 1 a 5).

dataset_com_indices_calculados.csv: Base de dados acrescida das colunas ISP, IAT e NSP (médias simples).

matriz_mapeamento_copsoq.md: Documento detalhando a relação entre os itens do questionário, os macro-fatores e os índices.

Como Reproduzir

Clone este repositório: git clone https://github.com/igorleorocha/copsoq_indicadores.git

Instale as dependências necessárias: pip install factor_analyzer pandas numpy scipy

Execute o script analise_fatorial_final.py no seu ambiente Python ou diretamente no Google Colab.

Aspectos Éticos e Limitações

Este estudo utiliza dados sintéticos. Não houve coleta de dados com seres humanos. Esta pesquisa constitui um primeiro passo exploratório e seus resultados sugerem uma base conceitual promissora, requerendo validação empírica futura em contextos organizacionais reais para a definição de pontos de corte e nexos causais.

Licença

Este projeto está licenciado sob a licença MIT.Contribuições e Contato:Sinta-se à vontade para abrir uma Issue ou enviar um Pull Request para melhorias metodológicas.
