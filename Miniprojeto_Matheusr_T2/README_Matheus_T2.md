Como executar este projeto:

1 - Este projeto foi desenvolvido no Google Colab.

2 - Faça o download do arquivo .ipynb deste repositório e abra-o no seu ambiente Google Colab.

3 - Conecte o seu Google Drive e certifique-se de que o arquivo Base Varejo.csv está no caminho indicado na primeira célula de código.

4 - Vá no menu superior do Colab, clique em "Ambiente de Execução" e depois em "Executar tudo".


1.  limpeza e Qualidade de Dados

P adronizei textos, ajustei as datas para o formato correto e tratei os espaços vazios usando estruturas condicionais. O meu objetivo aqui foi garantir que qualquer decisão tomada a partir deste projeto fosse baseada em relatórios estatísticos 100% confiáveis.

3. Como tratei e higienizei a base
Para transformar os dados brutos em informação limpa, executei os seguintes passos:

Leitura: Fiz a importação direta e estruturada do arquivo utilizando a biblioteca Pandas (read_csv) com o separador ;.

Tipagem: Converti a coluna de datas para o formato datetime64 e garanti que os IDs e a quantidade de filhos ficassem nos formatos numéricos corretos.

Limpeza: Fiz uma verdadeira faxina na base: eliminei 114.386 linhas duplicadas e excluí os poucos valores nulos numéricos residuais.

Condicionais: Criei uma função com a lógica if/else para varrer a base e substituir qualquer texto vazio ou nulo por "Sem Categoria" nas variáveis qualitativas.

3. O que descobri olhando para os dados (Principais Insights)
Com a casa arrumada, agrupei as informações e extraí as seguintes descobertas sobre a operação:

Perfil Familiar: A média matemática aponta 1.15 filhos por cliente, mas ao analisar a moda e a mediana (ambas em 0.0), comprovei que a grande maioria do nosso público não tem filhos cadastrados. Clientes com até 4 filhos são exceções no nosso banco de dados.

Comportamento por Gênero: Notei que o público feminino (F) é quem realmente lidera o volume de consumo, somando 382.427 transações e superando o público masculino (M), que registrou 351.019.

Carro-Chefe do Varejo: A categoria de Alimentos é o principal motor de vendas do negócio, dominando isolada no topo do ranking com 384.196 compras registradas.

Faturamento Complementar: Observei uma forte presença das categorias de Higiene (137.702) e Limpeza (128.632), que consolidam o segundo e o terceiro lugar em volume. Isso me mostra que o cliente aproveita a compra principal para já garantir os itens essenciais da rotina da casa.
