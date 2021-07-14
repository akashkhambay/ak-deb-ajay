# Akash-Deborah-Ajay
## API Documentation - Task

- SQL Database:
  - Change within in a Neighborbood is less likely to occur therefore it will be appropriate to use an SQL database as we predict it to contain data which is related to one another.
  - Reasoning for choosing an SQL database is further emphasised by the assumption that each household will have a unique id associated with them, this unique id could then be accessed in another table, which can be paired with the number of people in their household. See the example below.

|  Street Name   | Unique Id | House Owner |
| :------------: | :-------: | :---------: |
|  Coding road   |     1     |     Bob     |
| Javascript Ave |     2     |    Steve    |
| zebra stripes  |     3     |     Dan     |

    - As you can above the table has 3 columns with the middle column referring to the the unique id provided to the house owner on a particlar street in the neighbourhood.
    - This Unique Id could be used in another table to be linked to the postcode of the house, number of people in household etc...
    - Hence we feel it would be appropriate to make use of an SQL database, as the data is related in someway.

### Very basic Schema example of the SQL data and how it links

[API-Documentation.png](https://postimg.cc/Lnj1jbqr)

## Consideration of the Requests the API should be capable of handling:

- Every request to the neighbourhood API should be a GET request as the system is to only track people, houses and addresses in the neighbourhood.
- GET people living in the area and their information regarding age and name, the houses and addresses including post code, number of occupants in a house and owner of each house.
- There weren't be any changes that are made unless a resident moves out of the house, in which case we will use UPDATE and DELETE in order to update the records.
- POST request will send new data to the API to update the residential data whilst the DELETE request will remove data through the API.
