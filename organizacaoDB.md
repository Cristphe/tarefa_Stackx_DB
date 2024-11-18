O que devo fazer?

📍 Você foi convocado para um time que desenvolverá o novo Airbnb
Descreva como você organizaria um banco de dados que precisa , no inicio, de:

⏭️Usuários;
⏭️Lugares para se hospedar - cadastrados pelos usuários;
⏭️ Hospedagens (um período de tempo no qual usuário Y vai ficar no lugar X) - realizadas também por usuários;
⏭️ Avaliações feitas pelos usuários nas hospedagens.

📍 A descrição deve conter: 

⏭️ Nomes de tabelas que você faria;
⏭️ Colunas que você acha mais importantes nas tabelas;
⏭️ Relacionamentos delas e como ficaria nas colunas das tabelas;
⏭️ Uma explicação mínima de o que te levou por essas decisões

Tabelas:

pessoa
id 
razao_social 
cpf_cnpj 
data_nascimento
celular
email
senha
tipo_usuario 


lugares
id
pessoa_id
nome
descricao
endereco
valor_diaria

hospedes
id
lugar_id
usuario_id
data_inicio
data_final
valor_total
status

avaliacao
id
hospedagem_id
usuario_id
nota
comentario
data_avaliacao

Relações
pessoa --- lugares

lugares --- hospedes

pessoa -- hospedes

hospedes -- avaliação

Motivo das tabelas
Na tabela pessoa é onde fica todos os usuários, sendo um hospede ou anfitrião do lugar, sendo diferenciado por tipo pessoa.
Na tabela lugares é onde fica armazenado todos os locais que podem ser alocados, tendo o id do anfitrião e o que será mostrado na tela de busca de locais.
Na tabela hospedes é onde é feita a confirmação do local que o usuário quer, calculando o valor, trazendo as datas e se foi confirmado.
Na tabela avaliações é onde ficam as avaliações dos hospedes que já passaram por aquele local.
Separando as tabelas com os usuários cadastrados, locais fica de forma mais organizada e para facilita futuras consultas ao banco de dados, melhor também para o front puxar as informações que vão aparecer. Buscas mais rápidas e leves no sistema.

