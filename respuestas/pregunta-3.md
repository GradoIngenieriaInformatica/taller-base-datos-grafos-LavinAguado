MATCH (p:Persona)-[:AMIGO_DE]->(amigo)-[:VIVE_EN]->(c:Ciudad)
RETURN p.nombre, collect(DISTINCT c.nombre) AS ciudades_de_amigos;