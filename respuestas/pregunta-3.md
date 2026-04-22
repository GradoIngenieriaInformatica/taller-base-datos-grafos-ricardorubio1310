MATCH (p:Persona) OPTIONAL MATCH (p)-[:AMIGO_DE]-(amigo:Persona) RETURN p.nombre AS Persona, count(amigo) AS NumeroAmigos;
