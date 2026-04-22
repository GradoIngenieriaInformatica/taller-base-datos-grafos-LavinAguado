MATCH (p:Persona)-[:USA_TECNOLOGIA]->(t:Tecnologia)
RETURN p.nombre, COUNT(t) AS num_tecnologias;