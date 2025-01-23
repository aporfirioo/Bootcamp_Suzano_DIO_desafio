# Projeto Star Schema

## Descrição
Este projeto tem como objetivo construir um star schema baseado nos conceitos explorados durante o curso da DIO. O star schema é um modelo de dados que organiza tabelas de fatos e dimensões para facilitar consultas e análise de dados de forma eficiente.

## Estrutura do Star Schema
O star schema desenvolvido inclui as seguintes tabelas:

### Tabela de Fatos
- **Matriculado**
  - `Aluno_idAluno` (Chave Estrangeira)
  - `Disciplina_idDisciplina` (Chave Estrangeira)
  - `DataMatricula` (Data da matrícula)

### Tabelas de Dimensão
- **Dimensão Aluno**
  - `idAluno` (Chave Primária)
  - Outros detalhes dos alunos

- **Dimensão Disciplina**
  - `idDisciplina` (Chave Primária)
  - `Professor_idProfessor` (Chave Estrangeira)
  - Outros detalhes das disciplinas

- **Dimensão Curso**
  - `idCurso` (Chave Primária)
  - `Departamento_idDepartamento` (Chave Estrangeira)
  - Outros detalhes dos cursos

- **Dimensão Professor**
  - `idProfessor` (Chave Primária)
  - Outros detalhes dos professores

- **Dimensão Departamento**
  - `idDepartamento` (Chave Primária)
  - Outros detalhes dos departamentos

- **Dimensão Data**
  - `DataKey` (Chave Primária)
  - `Data`
  - `Dia`
  - `Mês`
  - `Ano`
  - `Trimestre`
  - `Semana do Ano`
  - `Dia da Semana`
  - `IsFeriado`
  - `IsFimDeSemana`
  - Outros detalhes relevantes

## Arquivos do Projeto
Os arquivos necessários para este projeto estão disponíveis no repositório:

1. **Arquivo do MySQL Workbench**: [star_schema_model.mwb](https://github.com/aporfirioo/Bootcamp_Suzano_DIO_desafio/blob/main/Desafio_04_PowerBI-starschema/star_schema_model.mwb)
2. **Imagem do Diagrama ER**: ![Diagrama ER]([link-para-imagem](https://github.com/aporfirioo/Bootcamp_Suzano_DIO_desafio/blob/main/Desafio_04_PowerBI-starschema/Diagrama%20ER.PNG))

## Instruções
1. Clone este repositório: `git clone https://github.com/seu-usuario/projeto-star-schema.git`
2. Abra o arquivo `star_schema_model.mwb` no MySQL Workbench para visualizar o modelo ER.
3. Utilize o script SQL gerado a partir do modelo para criar as tabelas no banco de dados.
4. Siga as melhores práticas de modelagem de dados e adapte conforme necessário para suas necessidades específicas.

## Contribuições
Sinta-se à vontade para dar um "fork" neste repositório e fazer suas alterações e melhorias. Toda contribuição é bem-vinda!


