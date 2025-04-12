### 🛒 Desafio Extra — Projeto de Vendas com PostgreSQL usando psycopg2 e ipython-sql.

Agora que você finalizou a análise dos dados de vendas, chegou o momento de estruturar tudo como um banco de dados relacional real!

Neste desafio, você irá:

✅ Conectar ao PostgreSQL  
✅ Criar as tabelas via SQL  
✅ Inserir os dados linha a linha a partir do DataFrame (o dataframe gerado da Venda o qual calculamos a venda com aumento) .
✅ Realizar algumas consultas de negócio com SQL puro  

---

#### 🎯 Objetivo

Transformar os dados do seu projeto de vendas em um banco PostgreSQL, criando uma tabela chamada `vendas_final`, contendo as informações abaixo:

##### 🧱 Estrutura esperada da tabela `vendas_final`

| Campo           | Tipo     | Descrição                            |
|-----------------|----------|--------------------------------------|
| cod_produto     | texto    | Código identificador do produto      |
| nome_produto    | texto    | Nome do produto                      |
| categoria       | texto    | Categoria do produto                 |
| valor_venda     | numérico | Valor original da venda              |
| venda_final     | numérico | Valor com aumento aplicado           |
| nome_vendedor   | texto    | Nome do vendedor responsável         |
| data_venda      | data     | Data em que ocorreu a venda          |

---

#### 🔌 Etapa 1 — Conectando ao banco PostgreSQL (Dica)

```python
import psycopg2

try:
    conn = psycopg2.connect(
        host="localhost",
        database="aula01",
        user="postgres",
        password="1234"
    )
    print("Conexão bem sucedida!")
except Exception as e:
    print("Erro ao conectar ao banco de dados:", e)

# Criar o cursor
crsr = conn.cursor()

```
#### 🔑 Etapa 2 — Crie as tabelas com SQL com Python;
#### 🔎 Etapa 3 - Inserir os dados na tabela apartir do dataframe.
#### 📥 Etapa 4 - Realizar algumas consultas de negócio com SQL puro.

- Qual foi o total de vendas por categoria?
- Quem foram os 3 vendedores que mais venderam?
- Qual a média de valor final de venda?


#### 📦 Entregáveis do Desafio:

✅ Notebook .ipynb com:

- Conexão via psycopg2;
- Criação da tabela vendas_final;
- Inserção linha a linha dos dados;
- Banco PostgreSQL populado com os dados corretos;
- Execução de 3 consultas SQL obrigatórias;

✅ Entrega do Projeto:

- Subir o projeto no GITHUB, documentado e me enviar o link do repositório por email.
- Ou enviar o projeto por e-mail: nayara.valevskii@gmail.com

#### DICA:

Aproveite o projeto para o portfólio, documente e post no Linkedin.

Boa sorte, galerinhaaa! 🔥

