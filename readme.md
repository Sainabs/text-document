1."height": "202",https://swapi.dev/api/people/4

2."population": "2000000000", https://swapi.dev/api/planets/2

3."manufacturer": "Corellian Engineering Corporation",https://swapi.dev/api/starships/10

4."name": "Droid" https://swapi.dev/api/species/2,  https://swapi.dev/api/people/2


5."films": 
           [ "title": "A New Hope", https://swapi.dev/api/films/1,
            "title": "The Empire Strikes Back","https://swapi.dev/api/films/2,
            "title": "Return of the Jedi",https://swapi.dev/api/films/3,
            "title": "The Phantom Menace",https://swapi.dev/api/films/4,
            "title": "Attack of the Clones",https://swapi.dev/api/films/5,
            "title": "Revenge of the Sith",https://swapi.dev/api/films/6
            ],


5.search query URL:https://swapi.dev/api/starships/?search=Millennium Falcon

part2
1. POST accepting a body "text": "",https://practiceapi.devmountain.com/api/posts
2. GET returns an array of all posts 
3. DELETE https://practiceapi.devmountain.com/api/posts/?id=555   

4. code: 409 Request query is missing required text property.

5. https://practiceapi.devmountain.com/api/posts
{
        "id": 75,
        "text": "Sainab",
        "date": "13 Jul 2022"
    },
6. https://practiceapi.devmountain.com/api/posts/?id=75
{
        "id": 75,
        "text": "Green",
        "date": "13 Jul 2022"
    },
7. https://practiceapi.devmountain.com/api/posts/filter/?text=blue
    [
        {
            "id": 74,
            "text": "blue",
            "date": "13 Jul 2022"
        },
        {
            "id": 67,
            "text": "MidnightBlue",
            "date": "13 Jul 2022"
        },
        {
            "id": 48,
            "text": "Blue",
            "date": "13 Jul 2022"
        },
        {
            "id": 36,
            "text": "blue",
            "date": "13 Jul 2022"
        },
        {
            "id": 25,
            "text": "Blue",
            "date": "13 Jul 2022"
        },
        {
            "id": 19,
            "text": "blue",
            "date": "13 Jul 2022"
        }
    ]
8. Content-Type: application/json; charset=utf-8

9. code: 409 Request was missing req.query.id or req.body.text

10. you get all the posts because it doesnt allow to input id query. it returns Code:200 Returns an array of all posts