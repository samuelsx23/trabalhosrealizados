UPDATE projetos   
SET status = 'Em andamento’;
CREATE TABLE desenvolvedores 
(  id INT AUTO_INCREMENT PRIMARY KEY,  
nome VARCHAR(100),  senioridade  
VARCHAR(30),  id_projeto INT,   
CONSTRAINT fk_projeto   
FOREIGN KEY (id_projeto)   
REFERENCES projetos(id
INSERT INTO desenvolvedores (nome, senioridade, id_projeto) VALUES  
 ('Ana Souza', 'Júnior', 1),   
('Bruno Lima', 'Pleno', 2),   
('Carla Mendes', 'Sênior', 3),   
('Diego Alves', 'Pleno', 4);
SELECT nome, orcamento FROM 
projetos   
WHERE linguagem = 'Python'  
 OR orcamento > 15000.00;
SELECT *   FROM projetos  
 WHERE nome LIKE 'Sistema%’;
SELECT   
 d.nome AS desenvolvedor, 
  d.senioridade,  
 p.nome AS projeto 
  FROM desenvolvedores d   
JOIN projetos p  
ON d.id_projeto = p.id;  
SELECT nome, orcamento   
FROM projetos  
 WHERE orcamento = (   
SELECT MAX(orcamento)   
FROM projetos
);
DROP TABLE IF EXISTS teste_tabelas;
SELECT    
p.nome AS projeto,    
COUNT(d.id) AS total_desenvolvedores   
FROM projetos p   
LEFT JOIN desenvolvedores d    
ON p.id = d.id_projeto   
GROUP BY p.nome;   
