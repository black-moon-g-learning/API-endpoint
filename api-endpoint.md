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