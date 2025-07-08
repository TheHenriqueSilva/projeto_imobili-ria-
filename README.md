Análise e Manipulação de Dados Imobiliários
Este repositório contém um projeto de análise de dados exploratória e manipulação de um dataset de imóveis para aluguel. O objetivo é demonstrar o uso da biblioteca pandas para tarefas comuns de ciência de dados, como importação, limpeza, filtragem e criação de novas features.

🚀 Funcionalidades
Importação de Dados: Carrega um dataset de imóveis diretamente de uma URL para um DataFrame do pandas.

Inspeção da Base de Dados: Verificação inicial das características gerais, como dimensões, nomes de colunas, tipos de dados e contagem de valores nulos.

Análise Exploratória:

Cálculo do valor médio de aluguel por tipo de imóvel.

Visualização da distribuição de preços por tipo de imóvel usando gráficos de barras.

Determinação do percentual de cada tipo de imóvel na base de dados.

Filtragem e Limpeza de Dados:

Remoção de imóveis comerciais para focar apenas em imóveis residenciais.

Tratamento de valores nulos, preenchendo-os com zeros.

Remoção de registros com valores inconsistentes (Valor ou Condominio iguais a zero).

Seleção de subconjuntos de dados com base em critérios específicos (ex: apartamentos com 1 quarto e aluguel menor que R$1200).

Criação de Novas Colunas:

Cálculo do Valor_por_mes (Valor + Condomínio).

Cálculo do Valor_por_ano (Valor por Mês * 12 + IPTU).

Criação de uma coluna Descricao combinando informações de Tipo, Bairro, Quartos e Vagas.

Adição de uma coluna categórica Possui_suite baseada na existência de suítes.

Exportação de Dados: Salva o DataFrame processado em um novo arquivo CSV.

📁 Estrutura do Projeto
Projeto_Imobiliaria.ipynb: O notebook Jupyter que contém todo o código para a análise e manipulação dos dados.

dados_apartamentos.csv: Arquivo CSV gerado após a filtragem inicial para conter apenas apartamentos.

dados_completos_dev.csv: Arquivo CSV final com os dados manipulados e as novas colunas criadas.

🛠️ Como Usar
Pré-requisitos
Para executar este projeto, você precisará ter o Python e as seguintes bibliotecas instaladas:

pandas

matplotlib (para as visualizações, embora não explicitamente importada no snippet, é comum para df.plot())

Você pode instalá-las usando pip:

Bash

pip install pandas matplotlib
Execução
Clone o repositório:

Bash

git clone https://github.com/TheHenriqueSilva/projeto_imobili-ria-.git
cd projeto_imobili-ria-
Abra o notebook Jupyter:

Bash

jupyter notebook Projeto_Imobiliaria.ipynb
Execute as células do notebook sequencialmente para replicar a análise e as transformações de dados.

📊 Fonte dos Dados
Os dados utilizados neste projeto são provenientes de um curso da Alura, acessados através da seguinte URL:
https://raw.githubusercontent.com/alura-cursos/pandas-conhecendo-a-biblioteca/main/base-de-dados/aluguel.csv

