# Casting Agency Specifications
The Casting Agency models a company that is responsible for creating movies and managing and assigning actors to those movies. You are an Executive Producer within the company and are creating a system to simplify and streamline your process.

# Getting Started

### Installing Dependencies

#### Python 3.9

# Models

Movies with attributes title and release date
Actors with attributes name, age and gender

### Endpoints
GET /actors and /movies
#### GET /actors

  - Fetch all the actors details.
  - Permission/Access given to : All


#### GET /movies

  - Fetch all the movies details.
  - Permission/Access given to :All


Optional:
#### GET /movies/<int:id>

  - Fetches movies details for a specific movie id 
  - Permission/Access given to : All


#### GET /actors/<int:id>

  - Fetches actor details for a specific actor id 
  - Permission/Access given to : All


DELETE /actors/ and /movies/
#### DELETE /actors/<int:id>

  - Deletes an actor for a specific actor id 
  - Permission/Access given to : Casting Director,Executive Producer.


#### DELETE /movies/<int:id>

  - Deletes a movie for a specific movie id 
  - Permission/Access given to : Executive Producer.


POST /actors and /movies and
#### POST /movies

  - Add a new movie 
  - Permission/Access given to : Executive Producer.


#### POST /actors
  - Add a new actor 
  - Permission/Access given to : Casting Director,Executive Producer.


PATCH /actors/ and /movies/
#### PATCH /actors/<int:id>
  - Update actor details for specifc actor id
  - Permission/Access given to : Casting Director, Executive Producer.



#### PATCH /movies/<int:id>
  - Update a movie for specifc movie id
  - Permission/Access given to : Casting Director, Executive Producer.



# Roles
Casting Assistant :
     Can view actors and movies
Casting Director :
    All permissions a Casting Assistant has and…
    Add or delete an actor from the database
    Modify actors or movies
Executive Producer :
    All permissions a Casting Director has and…
    Add or delete a movie from the database
# Tests
One test for success behavior of each endpoint
One test for error behavior of each endpoint
At least two tests of RBAC for each role



### DONE
