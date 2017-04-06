# roadhog
Fetch your api easily

## Utilisation d�sir�e: 
    Cas reel :
        - url : /api/mdv/practitioners?what=Medecin&where=nantes
        - url : /api/mdv/practitioners/1234/
        - url : /api/mdv/practitioners/1234/rdv/1
        - url : /api/mdv/specialties
    D�finition de l'url :
        D�port� dans REDUX :
            Cr�ation de REGEX pour r�cup�rer la resource voulu dans redux
        url direct : 
            Laisser la possibilit� de setter l'url en string directement
    Au travers de saga : 
        yield call(fetch, pathParam, queryParam, options, body)
    Direct :
        const resource = fetch('GET_RESOURCE')
        const ret = resource(pathParam, queryParam, options, body)

## Priorit�s :
OK  - 1) fetch resources simple
OK  - 2) ajouter le passage de parametre
OK  - 4) brancher redux
    - 5) gestion des options - besoin pour g�rer le same-origin
    - 6) g�rer les mocks
    - 7) ajouter un systeme de templating dans l'url de la resource
    - 8) gestion du body
