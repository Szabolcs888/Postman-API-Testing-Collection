# Postman API Testing Collection

![reqres_screenshot](https://github.com/user-attachments/assets/eb876e7c-7ca5-4877-8bdd-9d3539441b2f)


The repository was created as part of a practice project, which contains Postman collections (one for now, but will be expanded soon).

## Reqres API Test Collection

This Postman collection is for testing various endpoints of the [Reqres](https://reqres.in/) API. The collection includes tests for user management (CRUD operations), authentication, and error handling. It aims to demonstrate the basic principles of testing REST APIs using Postman. To run the tests, all you need to do is import the json file into Postman.

### Structure

The requests are grouped according to the following structure, organized into folders:
*   **Users:**
    *   `getUsers`: Retrieves a list of users.
    *   `getUserById`: Retrieves a user by ID.
    *   `createUser`: Creates a new user.
    *   `updateUser (PUT)`: Updates a user using the PUT method.
    *   `updateUser (PATCH)`: Updates a user using the PATCH method.
    *   `deleteUser`: Deletes a user.
*   **Authentication Tests:**
    *   `register`: Registers a new user.
    *   `registerUnsuccessful`: Tests unsuccessful registration.
    *   `registerUnsuccessfulEmptyBody`: Tests unsuccessful registration with an empty request body.
    *   `login`: Logs in with an existing user.
    *   `loginUnsuccessful`: Tests unsuccessful login.
    *   `loginUnsuccessfulEmptyBody`: Tests unsuccessful login with an empty request body.
*   **Error Handling Tests:**
    *   `getNonExistentUser`: Retrieves a non-existent user.
    *   `getNonExistentPage`: Retrieves a non-existent page.
*   **Performance Tests:**
    *   `delayedResponse`: Checks the response time for a delayed response.

### Variables

Variables are saved at the collection level, which can be modified as desired:
*   `baseUrl`: `https://reqres.in` (the URL of the Reqres API)
*   `userId`: `4` (the ID of an existing user)
*   `nonExistentUserId`: `32` (the ID of a non-existent user)
*   `page`: `2` (the page number for the `getUsers` request)
*   `delayTime`: `3` (the delay time for the `delayedResponse` request)
*   `email`: `eve.holt@reqres.in` (a user's email address)
*   `password`: `pistol` (a user's password)
*   `name`: `Eve` (a user's name)
*   `job`: `tester` (a user's job title)

#
#
<br>

# Postman API Testing Collection

A repository gyakorló projekt keretében jött létre, amely Postman collection-okat tartalmaz (egyelőre egyet, de hamarosan bővülni fog).

## Reqres API Test Collection

Ez a Postman collection a [Reqres](https://reqres.in/) API különböző endpointjainak tesztelésére szolgál. A collection tartalmazza a felhasználók kezeléséhez (CRUD műveletek), a hitelesítéshez és a hibakezeléshez szükséges teszteket. Célja, hogy bemutassa a REST API-k tesztelésének alapelveit a Postman használatával. A tesztek futtatásához nincs másra szükség, mint a json file Postmanbe való beimportálására.

### A tesztek csoportosítása

A kérések a következő struktúra szerint vannak csoportosítva, mappákba rendezve:
*   **Users:** A felhasználók kezeléséhez szükséges kérések (CRUD műveletek).
    *   `getUsers`: Lekérdezi a felhasználók listáját.
    *   `getUserById`: Lekérdez egy felhasználót az ID-ja alapján.
    *   `createUser`: Létrehoz egy új felhasználót.
    *   `updateUser (PUT)`: Frissít egy felhasználót a PUT metódussal.
    *   `updateUser (PATCH)`: Frissít egy felhasználót a PATCH metódussal.
    *   `deleteUser`: Töröl egy felhasználót.
*   **Authentication Tests:** A regisztrációval és a bejelentkezéssel kapcsolatos kérések.
    *   `register`: Regisztrál egy új felhasználót.
    *   `registerUnsuccessful`: Sikertelen regisztrációt tesztel.
    *   `registerUnsuccessfulEmptyBody`: Sikertelen regisztrációt tesztel üres kéréssel.
    *   `login`: Bejelentkezik egy létező felhasználóval.
    *   `loginUnsuccessful`: Sikertelen bejelentkezést tesztel.
     *   `loginUnsuccessfulEmptyBody`: Sikertelen bejelentkezést tesztel üres kéréssel.
*   **Error Handling Tests:** A hibás esetek teszteléséhez szükséges kérések.
    *   `getNonExistentUser`: Lekérdez egy nem létező felhasználót.
    *   `getNonExistentPage`: Lekérdez egy nem létező oldalt.
*   **Performance Tests:** A teljesítménytesztekhez szükséges kérések.
    *   `delayedResponse`: Ellenőrzi a response time-ot egy késleltetett válasz esetén.

### Változók

A változók collection szinten vannak elmentve, melyek tetszés szerint módosíthatók:
*   `baseUrl`: `https://reqres.in` (Reqres API URL-je)
*   `registeredUserId`: `4` (egy létező felhasználó ID-ja)
*   `nonExistentUserId`: `32` (egy nem létező felhasználó ID-ja)
*   `page`: `2` (az oldalszám a `getUsers` kéréshez)
*   `delayTime`: `3` (a késleltetés ideje a `delayedResponse` kéréshez)
*   `email`: `eve.holt@reqres.in` (egy felhasználó email címe)
*   `password`: `pistol` (egy felhasználó jelszava)
*   `job`: `tester` (egy felhasználó munkaköre)

