MATCH path = (p1:Persona)-[:AMIGO_DE*]->(p2:Persona)
WHERE ALL(r IN relationships(path) WHERE r.since > 2018)
RETURN path;