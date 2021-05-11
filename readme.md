# directus-101

## Getting started

### Default admin account

user: admin@example.com
pass: 1234

### Start

`yarn start`

Go to `http://localhost:8055/`

### Example

http://localhost:8055/items/titles

http://localhost:8055/presets/5

## Features

### filter

#### Show Fields

http://localhost:8055/items/titles?fields=id,status,test

#### Filter

http://localhost:8055/items/titles?filter[id][_eq]=2

#### Search (full text search)

http://localhost:8055/items/titles?search=ทดสอบ2

#### Sort

http://localhost:8055/items/titles?sort[]=sort&sort[]=-date_created

http://localhost:8055/items/titles?sort=sort,-date_created


#### Limit

http://localhost:8055/items/titles?limit=1

#### Offset (pagination)

http://localhost:8055/items/titles?offset=100

#### Page

* http://localhost:8055/items/titles?page=1
* http://localhost:8055/items/titles?page=2&limit=2

#### Metadata

* http://localhost:8055/items/titles?meta=total_count
* http://localhost:8055/items/titles?meta=filter_count
* http://localhost:8055/items/titles?meta=*

> https://docs.directus.io/reference/api/query/

## TODO List

* https://docs.directus.io/reference/api/query/#fields

### Note

https://docs.directus.io/reference/api/introduction/#rest-vs-graphql
