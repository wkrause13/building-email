FORMAT: 1A
HOST: https://building-email.com/api/

# building email

Building Email is a the api powering building-email.com

## Questions Collection [/users]

### List All Users [GET]

+ Response 200 (application/json)

        [
            {
                "email": "admin@building-email.com",
                "building": 23,
                "isAdmin": true,
                "created_at": "2015-08-05T08:40:51.620Z",
                "updated_at": "2015-08-05T08:40:51.620Z",
                "deleted_at": "",
            }
        ]

### Create a New User [POST]


+ Request (application/json)

        {
            "email": "admin@building-email.com",
            "password": "123445jsdf"
            "building": 23
        }

+ Response 201 (application/json)

    + Headers

            Location: /users/2

    + Body

            {
                "email": "admin@building-email.com",
                "building": 23,
                "isAdmin": true,
                "created_at": "2015-08-05T08:40:51.620Z",
                "updated_at": "2015-08-05T08:40:51.620Z",
                "deleted_at": "",
            }
