# PROJETO-INDIVIDUAL-MODULO-4
DIAGRAMA DO BANCO DE DADOS DA RESILIA


A Resilia está pensando em lançar um novo sistema de acompanhamento e para isso precisa de ajuda para modelar um
banco de dados que vai armazenar seus cursos, turmas e alunos.


-> Existem outras entidades além dessas três?

SIM, ALÉM DAS 3 ENTIDADES EXISTEM AS ENDITADES INSTITUÇÃO, INSTRUTORES, MATRICULA.
E 2 ENTIDADES ASSOCIATIVAS, COMO TURMA_INSTRUTORES E TURMA_ALUNOS.

-> Quais são os principais campos e tipos?
 
INSTITUIÇÃO: Endereço (varchar), nome (varchar), telefone (varchar), id_cnpj (pk/int).

CURSOS: curso_id(pk/int),requisitos (varchar), preco (varchar), id_cnpj (FK/INT).

TURMAS: data_final (date),curso_id(FK/int), id_turma (pk/int), horario (varchar), data_inicio (date

TURMA_INSTRUTORES: id_turma (FK/int),cpf_instrutores (FK/int), id_turma_instrutores (pk/int).

INSTRUTORES: nome (varchar), valor_hora (varchar), disciplina (varchar), email (varchar), cpf_instrutores (pk/int).

TURMA_ALUNOS: id_turma (FK/int), codigo_id (pk/int), cpf_aluno (FK/int).

MATRICULA: id_turma (FK/int), id_turma_aluno (pk/int), cpf_aluno (FK/int).

ALUNO: cpf_aluno (pk/int), data_nascimento (date), email (varchar), nome  (varchar).



-> Como essas entidades estão relacionadas?

 INSTUIÇÃO para varios CURSOS (1:1 E 1:N)
 
 CURSOS para TURMAS (1:1 E 1:N)
 
 TURMAS_INSTRUTORES (N:N)
 
 TURMAS_ALUNOS(N:N)
 
 TURMAS para MATRICULAS (1:1 E 1:N)

MATRICULA PARA ALUNO (1:1 E 1:1)
 
