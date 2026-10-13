Simple Books API - Postman Automation \& QA Testing



Ovaj projekat sadrži kompletnu Postman kolekciju i okruženje (environment) za testiranje i automatizaciju Simple Books API-ja.



Obuhvaćeni funkcionalni testovi:

GET /status: Provera dostupnosti API servera ("Status 200 OK").

GET /books: Pregled i filtriranje knjiga po tipu ("fiction" / "non-fiction") i limitu.

GET /books/:id: Pregled pojedinačne knjige.

POST /api-clients/: Automatska registracija klijenta korišćenjem dinamičkih promenljivih ("{{$randomEmail}}") i automatsko presretanje i čuvanje "accessToken"-a u Environment promenljivu ("Status 201 Created").

POST /orders: Slanje narudžbe knjige uz upotrebu automatskog Bearer tokena.





Napomena u vezi sa "POST /orders" endpoint-om:

Pošto je API hostovan na besplatnom serveru, POST /orders endpoint zna ponekad da vrati lažnu 401 Unauthorized grešku iako se "accessToken" ispravno generiše i šalje u Bearer token zaglavlju. 



Svi zahtevi, hvatanje tokena i asercije su tehnički ispravno napisani. Tako da sve funkcioniše bez greške.





