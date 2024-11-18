O que devo fazer?

🎯 Veja essa tabela e escreva a query pedida no fim:

Tabela - provas
📍Colunas:
📍 id_aluno  - número
📍 id_materia  - número
📍 nota  - número flutuante
📍 data_da_prova  data

Tabela - aluno
📍 colunas:
📍 id numero
📍 nome string
📍 data_nascimento numero

Tabela - professor
📍 colunas:
📍 id numero
📍 nome string
📍 data_nascimento numero

Tabela - materia
📍 colunas:
📍 id numero
📍 nome string
📍 id_professor numero


🎯 Crie 3 alunos;
🎯 Crie uma matéria e um professor;
🎯 Crie 1 prova para cada aluno nessa matéria e diga que nota eles tiraram.

Vamos levar em consideração o PostGre pois é o que eu utilizo atualmente.

INSERT INTO aluno (id, nome, data_nascimento) VALUES
(1, 'Cristophe', '2005-03-15'),
(2, 'Damião', '2002-01-29'),
(3, 'Junior', '1995-04-29')

INSERT INTO professor (id, nome, data_nascimento) VALUES
(1, 'João', '1975-06-18')

INSERT INTO materia (id, nome, id_professor) VALUES
(1, 'Programação', 1)


INSERT INTO provas (id_aluno, id_materia, nota, data_da_prova) VALUES
(1, 1, 6.0, '2024-11-18'),
(2, 1, 8.5, '2024-11-18'),
(3, 1, 7.3, '2024-11-18')
