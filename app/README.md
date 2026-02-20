1. Usuarios admin (alcaldes, gobernadores, senadores, presidentes, etc)
2. Usuarios Seguidores (personas que inscriben posibles votantes)

## Flujo.

1. el usuario admin se registra.

interface UserCandidato{
    id,
    name,
    postulacion (alcalde, presidente, etc...),
    idCampaña,
    votantes team[],
    partido
} 

2. uno de sus seguidores se registra para buscar posibles votantes.

iterface UserSeguidor{
    id,
    name,
    idCampaña,
    team: votantes[] 'personas que lo siguen'
    partido.
}

3. se registran todos los posibles votantes (los votantes solo pueden estar en un grupo)

interface Votante{
    id,
    name,
    cedula,
    direccion,
    edad,
    seguidor.
    partido.
}

## Administracion

# los administradores podran ver:
1. numero de posibles votantes
2. sectores en un mapa con los votantes
3. edad media de los votantes

# Los seguidores podran:
1. Unirse a un candidato
2. registrar votantes
3. ver una lista de sus seguidores