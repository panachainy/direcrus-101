# directus-101

## Todo

* [try relation and translation](https://docs.directus.io/concepts/translations/#schema-translations)

translation.*

## Getting started

### Default admin account

user: admin@example.com
pass: 1234

## Start

`yarn start`

Go to `http://localhost:8055/`

### Example

http://localhost:8055/items/formula

## Features

### filter

#### Show Fields

http://localhost:8055/items/formula?fields=id,key

#### Filter

http://localhost:8055/items/formula?filter[id][_eq]=2

#### Search (full text search)

http://localhost:8055/items/formula?search=FORMULA_CI_GOAL

#### Sort

http://localhost:8055/items/formula?sort[]=id&sort[]=-created_at

http://localhost:8055/items/formula?sort[]=id

http://localhost:8055/items/formula?sort[]=-id

http://localhost:8055/items/formula?sort=sort,-created_at

#### Limit

http://localhost:8055/items/formula?limit=1

#### Offset (pagination)

http://localhost:8055/items/formula?offset=7&meta=*

http://localhost:8055/items/formula?offset=3

#### Page

* http://localhost:8055/items/formula?page=1
* http://localhost:8055/items/formula?page=2&limit=4&meta=*

#### Metadata

* http://localhost:8055/items/formula?meta=*

> https://docs.directus.io/reference/api/query/

## Concern

* not have count per page in metadata

### Note

https://docs.directus.io/reference/api/introduction/#rest-vs-graphql

## auth

POST http://localhost:8055/auth/login

{
	"email": "admin@example.com",
	"password": "1234"
}

token: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjE0ZDU2NTZhLWJiZTctNDU1ZC1hMzA4LTdkZWYyZDM2MzM3MiIsImlhdCI6MTYyMDcyMzYyNiwiZXhwIjoxNjIwNzI0NTI2fQ.ner4jx6QdWzFHT_hn-IRrUAQZgnJvdMPve4TSgJk2Cw

### Access to graphql playground *not work or not have
* https://github.com/directus/directus/issues/3796
* https://github.com/directus/directus/issues/4264

> http://localhost:8055/graphql?access_token=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjE0ZDU2NTZhLWJiZTctNDU1ZC1hMzA4LTdkZWYyZDM2MzM3MiIsImlhdCI6MTYyMDcyMzYyNiwiZXhwIjoxNjIwNzI0NTI2fQ.ner4jx6QdWzFHT_hn-IRrUAQZgnJvdMPve4TSgJk2Cw
