# Desafio: criando um pipeline para ETL.

## Contexto

Nesse projeto, serão utilizados dados do IBGE de população estimada em cada cidade. O objetivo é simular um processo de ETL da seguinte forma:

**Extração**: leitura de uma planilha contendo as informações de cada município e sua população estimada;

**Transformação**: baseando-se na população estimada, classificar a cidade em **pequeno porte**, **médio porte** ou **grande porte**;

**Carregamento**: carregar as informações para uma tabela no PostgreSQL.

Para a classificação, será considerado o seguinte cenário:

| População | Classificação |
| - | - |
| Até 50.000 | Pequeno Porte |
| Entre 50.000 e 100.000 | Médio porte |
| Acima de 100.000 | Grande porte |

O código foi desenvolvido na linguagem python, utilizando o terminal.

Para a conexão entre o terminal e o servidor do Postgre, é necessário configurá-lo para receber conexões.

As bibliotecas utilizadas estão listadas abaixo:
- pandas
- create_engine from sqlalchemy

Para formatação do código, foi utilizado um notebook do Google Colab, que foi exportado para o Github.


### Documentos
- [Planilha_Dados do IBGE](IBGE_POP2021_20220207.xls)
- [Código_Google Colab](DIO_Pipeline_ELT.ipynb)