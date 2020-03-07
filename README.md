# PlateSlate
## Setup
1. ```mix deps.get```
2. ```mix ecto.setup```

## GraphQL
GraphQL is a query language that gives the users of an API the ability to describe the data that they want, and lets creators of the API focus on data relationships and business rules instead of worrying about the various data payloads the API needs to return.

### Problems with REST
As a client of this REST API, you have very limited control over what is returned. The contract between the client and the server is fairly one- sided: the client gets what the server wants to give it.

REST API authors attempting to address this problem use a number of differ- ent techniques and conventions:
* Writing detailed, custom documentation about API responses, so clients at least know what to expect
* Supporting query parameters (like include and fields) that act as flags to select information, adding some limited flexibility
* Including references (either IDs or URLs) to related data, rather than embedding it, effectively splitting the query across multiple requests
* Using different resources to model different levels of data inclusion (for example, /users/123 as a full set of data and /profiles/123 as a sparse set of data), duplicating or reusing large chunks of code
* Splitting the API completely, perhaps by platform (for instance, exposing /desktop/users/123 and /mobile/users/123), to support the needs of different types of clients
* Some combination of all of these

REST’s simplicity falls away pretty suddenly as the needs of clients become more varied and the surface area of the API expands.

# Upto

Page 30

Our Schema Module

Before that: explore the postgresql database and get familiar with the dataset
