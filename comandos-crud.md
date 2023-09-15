# Comandos SQL - Para CRUD (Referencia)

### Resumo

C -> Create (Insere dados)
R -> Read (Ler dados)
U -> Update (Atualizar dados)
D -> Delete (Apaga dados)

## Insert
## Fabricantes

```sql

INSERT INTO fabricantes (nome) VALUES ('Asus')
INSERT INTO fabricantes (nome) VALUES ('DELL')
INSERT INTO fabricantes (nome) VALUES ('Apple'), ('LG'), ('Samsung'), ('Brastemp')
```

## Insert
## Produtos

```sql
INSERT INTO produtos (nome, descricao, preco, quantidade, fabricante_id)
VALUES('Ultrabook', 'Ultrabook Asus Intel Core I9', 6500.99, 7, 1);

INSERT INTO produtos (nome, descricao, preco, quantidade, fabricante_id)
VALUES('Geladeira', 'Frost-Free com acesso a internet', 8500.99, 10, 6);

INSERT INTO produtos (nome, descricao, preco, quantidade, fabricante_id)
VALUES('Tablet Android', 'Tablet 10 Polegadas com 256Gb de armazenamento', 4900.99, 3, 5);

INSERT INTO produtos (nome, descricao, preco, quantidade, fabricante_id)
VALUES('Asus Zenfone 9', 'Celular ultracompacto, ultraelegante e ultrarrápido', 4500.99, 4, 1);

INSERT INTO produtos (nome, descricao, preco, quantidade, fabricante_id)
VALUES('Xbox', 'Console de ultima geração', 2500.00, 6, 8);

INSERT INTO produtos (nome, descricao, preco, quantidade, fabricante_id)
VALUES('Ultrabook', 'AMD Ryzen 5 16Gb RAM', 4500.99, 3, 7);

```

## Insert
## Fabricantes

```sql
INSERT INTO fabricantes (nome) VALUES ('Positivo'), ('Microsoft');
/```