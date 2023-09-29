## Referencia

sql
CREATE DATABASE cinema CHARACTER SET utf8mb4;

 

sql
CREATE TABLE filmes(

    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    titulo VARCHAR(45)
    lançamento YEAR(4)
)




sql

CREATE TABLE generos(

    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    genero VARCHAR(45)

)



### Adicionar Campo/Coluna em uma Tabela

sql
ALTER TABLE filmes ADD genero_id INT NOT NULL
AFTER lancamento



sql
ALTER TABLE filmes
ADD CONSTRAINT fk_filmes_generos

FOREIGN KEY(genero_id) REFERENCES generos(id)


sql

INSERT INTO generos (nome)
VALUE ('Ação'), ('Comédia'), ('Drama'), ('Romance'), ('Suspense'), ('Terror'), ('Ficção Científica')



sql

INSERT INTO filmes(titulo, lancamento, genero_id)
VALUE ('Star Wars: Episódio III – A Vingança dos Sith ', 
2005,
7
);

INSERT INTO filmes(titulo, lancamento, genero_id)
VALUE ('A Freira', 
2018,
6
);

INSERT INTO filmes(titulo, lancamento, genero_id)
VALUE ('Para Todos os Garotos que já Amei', 
2018,
4
);

INSERT INTO filmes(titulo, lancamento, genero_id)
VALUE ('A Queda', 
2022,
5
);
