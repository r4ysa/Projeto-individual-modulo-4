# Projeto-individual-modulo-4

O banco de dados pensado para o novo sistema de acompanhamento da resilia foi organizado para armazenar dados de professores, alunos, turmas e cursos.

- Entidades:

Primeiramente foi criado novas entidades além das três sugeridas, sendo elas endereço e professor. A escolha da criação da entidade endereço foi justamente por conta da quantidade de informações necessárias, logo fica mais organizado guardar esses dados separadamente numa tabela específica. A entidade professor foi criada pois se relaciona diretamente com a turma e curso, assim consequentemente com os alunos. Portanto, com as novas entidades criadas o sistema da empresa fica mais completo e funcional contendo informações mais detalhadas. 

- Tabelas:

. A tabela aluno tem como colunas as informações básicas para efetuação da matrícula, como nome, telefone e CPF. Foi optado pelo CPF ser a chave primária, uma vez que é um registro único.    

. A tabela professor tem o mesmo objetivo da tabela aluno, ou seja, armazenar dados para que se tenha um registro dos professores que irão ministrar as aulas. Novamente o CPF foi escolhido como chave primária pelo mesmo motivo citado anteriormente.

. A tabela endereço contém colunas para serem preenchidas com os dados dos professores ou alunos ao realizarem suas matrículas/registros. Possue campos como rua, CEP e número. Para a chave primária, foi criado um campo idEndereço para ser um registro único.

. A tabela curso têm as colunas que guardarão informações suficientes para os mesmos serem oferecidos ao público alvo. Alguns campos são nome, duração e categoria. A chave primária é o nome pois não existirá mais de um curso com mesma nomeação, logo o nome é único.

. A tabela turma contém como campos nome, data de início e quantidade de alunos. Foi criado um campo idTurma para ser um registro único da mesma.

. Os principais tipos de campos utilizados foram varchar, char, int e date.

- Relacionamentos:

. Cada aluno/professor possui apenas um endereço e cada endereço é referente à um aluno/professor. Relacionamento 1:1.

. Cada aluno pode estar matriculado em vários cursos e consequentemente várias turmas também. Assim, mais de uma turma ou curso pode ter este aluno. Relacionamento 1:n.

. Um curso pode ter várias turmas, logo várias turmas poderão ser referentes à um mesmo curso. Relacinamento 1:n.

. Várias turmas poderão ter vários professores. Relacionamento n:m. 
