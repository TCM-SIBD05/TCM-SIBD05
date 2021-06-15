# C3 : SQL

## DDL

```sql
create database pingo_salgado;
use pingo_salgado;


CREATE TABLE IF NOT EXISTS `funcionario` (
`idFuncionario` int NOT NULL auto_increment PRIMARY KEY,
`nome` text NOT NULL,
`idade` int(3) unsigned NOT NULL,
`sexo` ENUM('m','f') NOT NULL,
`salario` int(7) unsigned NOT NULL,
`entrada` time,
`saida` time,
`seccao` int(2) unsigned NOT NULL,
`classe` varchar(15) NOT NULL,
`escala` varchar(15) NOT NULL
);

CREATE TABLE IF NOT EXISTS `formacao` (
`idFormacao` int NOT NULL auto_increment PRIMARY KEY,
`nome` varchar(20) NOT NULL
);

CREATE TABLE IF NOT EXISTS `func_form` (
`idFunc_Form` int NOT NULL auto_increment PRIMARY KEY,
`idFunc` int NOT NULL,
`idForm` int NOT NULL,
FOREIGN KEY (idFunc) REFERENCES funcionario(idFuncionario) ON DELETE cascade ON UPDATE cascade,
FOREIGN KEY (idForm) REFERENCES formacao(idFormacao) ON DELETE cascade ON UPDATE cascade
);
```

---
[< Previous](rebd04.md) | [^ Main](https://github.com/TCM-SIBD05/TCM-SIBD05) | Next >
:--- | :---: | ---: 