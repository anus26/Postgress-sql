CREATE TABLE HOMEITEMS(
ID SERIAL PRIMARY KEY,
HOMEITEMS VARCHAR(800),
price DECIMAL (3,0),
Genre VARCHAR (100),
AVALIABLE BOOLEAN
)

SELECT * FROM Homeitems

INSERT INTO Homeitems(
homeitems,price,genre,avaliable
) VALUES
(
'knife',120.00,'REQUIRED',TRUE
),
(
'Boxes',500.00,'REQUIRED',TRUE
),
(
'Italian glass',110.00,'REQUIRED',TRUE
)

SELECT * FROM Homeitems
Where Homeitems LIKE '%glass'

SELECT * FROM Homeitems
Where  price < 300

SELECT * FROM Homeitems
ORDER BY PRICE DESC

SELECT * FROM Homeitems
Where Genre LIKE 'Italian glass'

SELECT * FROM Homeitems
Where Avaliable = False

DELETE FROM Homeitems
where Homeitems='knife'

UPDATE Homeitems
SET avaliable=False
where  Homeitems='bottles'

