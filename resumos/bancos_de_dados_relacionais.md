
# 👨‍💻 BANCOS DE DADOS RELACIONAIS


## Estrutura de um Banco de Dados Relacional
- Relacionamento entre as tabelas
- Linguagem de Consulta Estruturada (SQL)
- Integridade Referencial (Não permite deletar uma tabela que tenha dados dependendtes em outra tabela)
- Normalização de dados 
- Segurança (Configuração de acesso a determinadas partes dos dados para determiandas pessoas)
- Flexibilização e Extensibilidade
- Suporte a transações ACID (Garantia da consistencia do banco de dados)

#### ACID
- Atomicidade: Se alguma alteração em cadeia de errado, a primeira alteração é revertida ao estado anterior. 
- Consistência: Saída de um estado consistente para outro estado consistente. Para que seja alterado um dado por exemplo, ele precisar respeitar as regras do tipo do dado e as obrigatoriedades daquela coluna.
- Isolamento: Uma alteração feita ela compete apenas uma por vez (sem ser feita ao mesmo tempo para não haver perda.
- Durabilidade: Alteração permanente

## Conceitos Básicos ao SQL (STRUCTURED QUERY LANGUAGE)

- DQL (Consulta de Dados) -> SELECT
- DML (Manipulação de Dados) -> INSERT, UPDATE e DELETE
- DDL (Definição de Dados -> Tipos, onde vao ser armazenados, etc
-> CREATE, ALTER e DROP

## MER (Modelo Entidade- Relacionamento) -> DER (Diagrama Entidade-Relacionamento)
- Criar grafos DER: https://app.quickdatabasediagrams.com/#/
- Entidades -> Nomes das Planilhas (Entity/Quadrado)
- Atributos -> Colunas da Planilha (Atribute Area/Oval)
- Relacionamentos -> Associações entre as entidades (Losangulo)

#### Cardinalidade

- Um-para-Um (1:1): Cada instância de uma entidade se relaciona com no máximo uma única instância de outra entidade, e vice-versa. Exemplo: Pessoas e CPFs em um sistema de RH.
- Um-para-Muitos (1:N): Cada instância de uma entidade se relaciona com muitas instâncias de outra entidade, mas não vice-versa. Exemplo: Cursos e Aulas.
- Muitos-para-Muitos (N:M): Muitas instâncias de ambas as entidades se relacionam umas com as outras. Exemplo: Alunos e Cursos.
- Zero-ou-Um-para-Muitos (0..1:N): Uma instância de uma entidade pode se relacionar com nenhuma ou no máximo uma única instância da outra entidade, mas cada instância dessa outra entidade pode se relacionar com muitas da primeira. Exemplo: Funcionários e Gerentes em uma empresa. 