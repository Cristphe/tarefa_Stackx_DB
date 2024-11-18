O que devo fazer?

Crie uma tabela fictícia e depois faça uma query para cada item de um CRUD - Criar uma linha, selecionar(ler), editá-la e apaga-la.

CREATE TABLE item (
 id PRIMARY KEY,
 nome VARCHAR(100) NOT NULL,
 qtd INTERGER NOT NULL
)

INSERT INTO item(id, nome, qtd)
VALUES (1, 'Notbook', 10)

SELECT * FROM item WHERE id = 1

UPDATE item
SET qtd = 15
WHERE id = 1

DELETE FROM item WHERE id = 1
