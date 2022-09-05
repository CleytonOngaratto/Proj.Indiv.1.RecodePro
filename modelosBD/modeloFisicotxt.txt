create table destino(
id_destino int auto_increment,
cidade varchar(20),
valor float,
primary key (id_destino)
);

create table promocao(
id_promocao int auto_increment,
nome varchar(30),
desconto float,
destino int ,
foreign key (destino) references destino(id_destino),
primary key (id_promocao)
);
