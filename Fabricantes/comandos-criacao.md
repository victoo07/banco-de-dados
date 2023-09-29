# Comandos SQL - Referência

## Modelagem física

### Criar banco de dados

```sql

CREATE DATABASE vendas CHARACTER SET utf8mb4;

```

### Criar a tabela fabricantes

```sql
CREATE TABLE fabricantes (
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL
)
```

### Criar a tabela produtos

```sql
CREATE TABLE produtos (
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL,
    descricao TEXT(1000) NOT NULL,
    preco DECIMAL(6,2) NOT NULL,
    quantidade TINYINT(4) NOT NULL
)
```
### Inserir campo/coluna na tabela

```sql

ALTER TABLE produtos ADD fabricante_id INT NOT NULL
AFTER quantidade;

```
### Criação da chave estrangeira

```sql

ALTER TABLE produtos
ADD CONSTRAINT fk_produtos_fabricantes
FOREIGN KEY(fabricante_id) REFERENCES fabricantes(id)

```

