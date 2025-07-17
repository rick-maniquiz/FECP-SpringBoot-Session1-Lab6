# Spring Boot Session 1 Lab 6

#### By: Rafael Nico T. Maniquiz

## Endpoints

**Resources:**
1. Zoo
2. Admin
3. Handler
4. Vendor
5. Veterinarian
6. Visitor
7. Ticket
8. Shop
9. Products
10. Enclosure
11. Specie
12. Animal
13. Hospital
14. SickAnimal
15. HealedAnimal


| Method | URL | Purpose |
|--------|-----|---------|
| POST | /admins | when admins are logging in, verify the credentials |
| PATCH | /admins/{adminID}/zoo | admins closing or opening the zoo (modifying open status) |
| POST | /admins/{adminID}/zoo/enclosures | admins configuring the available enclosures |
| POST | /admins/{adminID}/zoo/enclosures/{enclosureID}/species | admins configuring the available animals per enclosure |
| POST | /admins/{adminID}/zoo/enclosures/{enclosureID}/species/{specieID}/animals | admins configuring the available animals per enclosure |
| POST | /admins/{adminID}/zoo/enclosures/{enclosureID}/handlers | admins assigning handlers for the enclosures |
| POST | /admins/{adminID}/zoo/shops | admins configuring the available shops |
| POST | /admins/{adminID}/zoo/shops/{shopID}/vendors | admins assigning vendors for the available shops |
| POST | /admins/{adminID}/zoo/hospital | admins configuring the hospital |
| POST | /admins/{adminID}/zoo/hospital/veterinarians | admins assigning veterinarians in the hospital |
| GET | /zoo/handlers/{handlerID}/enclosures/{enclosureID}/species/{specieID}/animals | handler viewing animals in the enclosure they handle |
| POST | /zoo/handlers/{handlerID}/enclosures/{enclosureID}/species/{specieID}/animals/{animalID} | handler feeding/exercising the animal |
| POST | /zoo/handlers/{handlerID}/hospital/sickAnimals | handler sending the animal to the hospital |
| POST | /zoo/visitors | adds a visitor to the visitors in a zoo |
| POST | /zoo/visitors/{visitorID}/tickets | visitors buying tickets |
| GET | /zoo/visitors/{visitorID}/tickets | viewing all valid tickets |
| GET | /zoo/shops | view available shops |
| GET | /zoo/shops/{shopsID} | visiting a shop |
| GET | /zoo/shops/{shopsID}/products | viewing shop products |
| POST | /zoo/shops/{shopsID}/vendors/{vendorID}/products/{productsID} | buying/selling an item in the shop |
| GET | /zoo/enclosures/species | viewing which specie enclosures to visit |
| GET | /zoo/enclosures/species/{specieID}/animals | viewing all the animals in the specific specie enclosure |
| POST | /zoo/enclosures/species/{specieID}/animals/{animalID} | feeding a specific animal from the enclosure |
| POST | /zoo/hospital | visit a hospital |
| GET | /zoo/hospital/healedAnimals | view all healed animals in the hospital |
| GET | /zoo/hospital/sickAnimals | view all unhealthy animals in the hospital |
| DELETE | /zoo/hospital/sickAnimals | the veterinarian of the hospital heals all the animals |
| POST | /zoo/hospital/veterinarians/{veterinarianID} | the veterinarian of the hospital gives a lecture |
| DELETE | /zoo/visitors | adds a visitor to the visitors in a zoo |
