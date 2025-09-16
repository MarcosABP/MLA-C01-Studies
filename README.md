# 📘 MLA-C01-Studies
## Estudos práticos envolvendo assuntos abordados no exame AWS Certified Machine Learning Engineer Associate (MLA-C01)
## ℹ️ ** A explicação dos códigos explicados dos estudos abaixo estão todos disponíveis nos notebooks.

## TF-IDF

Esta seção mostracomo aplicar o TF-IDF (Term Frequency – Inverse Document Frequency) na prática, usando Amazon EMR com PySpark 

TF (Term Frequency) → frequência de um termo dentro de um documento.
IDF (Inverse Document Frequency) → diminui a importância de termos muito comuns e aumenta o peso de termos incomuns.
TF-IDF = TF × IDF → vetor numérico que representa a importância de cada palavra em cada documento.

### Configuração AWS

Antes de executar o código, devem ser feitas algumas configurações no ambiente AWS. 

1. Abra a aba de Amazon EMR, e e acesse a seção de "Studios", onde é criado um ambiente de notebook PySpark interativo. Na criação de um Studio, é criado também um bucket S3, que é usado para armazenamento do workspace padrão de um Studio EMR.
2. Nomeie e crie a instância
3. Ao concluir, um notebook jupyter é aberto, onde podemos rodar nosso código.

### Código
1. No notebook do EMR Studio, faça upload do arquivo .ipynb disponível na pasta TF-IDF-EMR.
2. Selecione o kernel PySpark no notebook.
3. Execute as células do código para rodar o pipeline:
- Tokenização do texto
- HashingTF para gerar as frequências
- IDF para calcular os pesos
- TF-IDF final armazenado na coluna features

