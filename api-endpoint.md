# API endpoints # 

## Host ##

```
https://g-learning.click/

```
1. GET continents
   
   a. endpoint
    ```
    https://g-learning.click/api/continents
    ```
    b. params

        null

    c. response

        array
    d. method

        GET

2. GET countries in a continents
   
    a. endpoint

    ```
    https://g-learning.click/api/continents/{id}

    ```
    b. params

        id ->integer

        example: 1,2

    c. response

        array with popular and countries

    d. method

        GET

3. GET topic of a country
   
    a. endpoint

    ```
    https://g-learning.click/api/countries/{id}/topics
    ```
     b. params

        id ->integer

        example: 1,2

    c. response

        array
    d. method

        GET

4. GET videos of a country topic

    a. endpoint

        https://g-learning.click/api/countries-topics/{id}/videos
    b. params

        id ->integer

        example: 1,2

    c. response

        array
5. Login 
   
    a. endpoint

        https://g-learning.click/api/login
    
    b. params
    
        username: fasfdsdfdsfdsf
        password: 123456789
    c. response

        array

        {
            "message": "success",
            "data": {
                "status": true,
                "token": "4|VCL67xahQpnBQ1GsnoJ1hBOnOJ4vB58UjPxrwLke",
                "type": "Bearer Token"
            }
        }

    d. method

        POST
6. Register
   
    a. endpoint

        https://g-learning.click/api/register
    b. params

        [
            username,
            password,
            password_confirm,
            phone
        ]
    c. response

        array
    d. method

        POST
    e. Example

    ![alt text](./assets/Screenshot%20from%202023-02-05%2016-33-43.png)

7. Search
    
    a. endpoint

        https://g-learning.click/api/countries-topics/{id}/videos?s={search}
    b. params

        id -> integer
        search-> string
    c. response

        array
    d. example

    ![alt text](assets/Screenshot%20from%202023-02-06%2017-10-59.png)

    e. method

        GET
    f. note

        Please need to search from 2 symbols

8. Get information in maybe you don't know
   
    a. endpoint

        https://g-learning.click/api/information

    b. param
    
        null

    c. response

        an array with paginate

    d. example

    ![alt text](assets/information.png)
    
9. Get services information

    a. endpoint

        https://g-learning.click/api/services
    b. response 

        {
            "message": "success",
            "data": [
                {
                "id": 1,
                "name": "Damien McCullough",
                "description": "https://via.placeholder.com/640x480.png/00cc00?text=animal+iusto",
                "price": 17000,
                "unit": "VND",
                "image": "https://via.placeholder.com/640x480.png/00cc00?text=animal+iusto"
                }
            ]
        }
10. Get levels of games

    a. endpoint 

        https://g-learning.click/api/levels
    b. METHOD

        GET
    c. response
    ![alt text](./assets/levels.png)
11. Get list countries
    
    a. endpoint

        https://g-learning.click/api/countries?page={page}
    b.method

        GET

    c. param

        page -> integer
    d. response
    ![alt text](./assets/list-country-history.png)
12. Get list question in a country(Game lv 1) 
    
    a. endpoint 

        https://g-learning.click/api/countries/{id}/questions
    b. method
        
        GET
    c. param

        id->integer
    d. response

    ![alt text](assets/list-question-in-country.png)
13. Create new history when user play game

    a. endpoint

        https://g-learning.click/api/countries/user-play-game
    b. method

        POST
    c. example

    ![alt text](assets/create-history.png)

14. Search Countries

    a. endpoint 

        https://g-learning.click/api/continents/{id}?s={text}
    b. method

        GET
    C. example
    ![alt text](assets/search-country.png)
    
15. Error when expired trail days
    
    a. endpoint

        Every  endpoints without: 
            + payment
            + profile (include update profile)
    b. method

        GET
    c. example
    ![alt text](assets/error-expired-trial-days.png)

16. Store data after user play game

    a. endpoint 

        https://g-learning.click/api/countries/{id}/history-play-game
    b. method

        POST
    c. param
    
        id->integer
        total_questions->integer| grater than total_correct_answers
        total_correct_answers->integer
    d. example 
    ![alt text](assets/history-play-game.png)

17. Get review question
    
    a. endpoint

        https://g-learning.click/api/videos/{id}/questions
    b. method

        GET
    c. param

        id->integer

    d. example

    ![alt text](assets/review-2.png)
18. Search countries in  game page
     a. endpoint 

        https://g-learning.click/api/countries?s={text}
    b. method

        GET
    C. example
    ![alt text](/assets/search-countries.png)
    
