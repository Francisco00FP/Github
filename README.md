CREATE TABLE Jogoss (
    Codigo INT IDENTITY(1,1) PRIMARY KEY, 
    Nome VARCHAR(100),
    Data_Lancamento varchar(10),
    Valor float
);

Alter table jogoss
add Avaliação varchar(10);


INSERT INTO Jogoss (Avaliação)
WHERE Codigo BETWEEN 1 AND 20
VALUES
('9.5/10'),
('7.5/10'),
('10/10'),
('9.5/10'),
('8/10'),
('9/10' ),
('9/10'),
('9/10' ),
('8.5/10'),
('9.5/10'),
('9/10'),
('9/10'),
('7/10'),
('8.5/10'),
('9/10'),
('9.5/10'),
('9/10'),
('8.5/10'),
('9/10'),
('7.5/10');



select *
From Jogoss


UPDATE Jogoss
SET Avaliação ='7.5/10',
WHERE Codigo = 2;


DELETE FROM Jogoss
WHERE Codigo BETWEEN 21 AND 60;
