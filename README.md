# Complete collection of Motum's API services

### To run this bad boi
Install docker you douche, and then

```shell
docker-compose up
```

But before you do that, make sure you provide (either through `.env` file or by pre-populating your environment) following environment variables
- `ACCESS_TOKEN_SECRET` - token used to sign access tokens provisioned by an API
- `REFRESH_TOKEN_SECRET` - token used to sign refresh tokens provisioned by an API
- `DATABASE_URL` - posrgress URL to a database in format: 
`postgresql://<username>:<password>@<hostname>:<port>/<database>?schema=<schema_name>`
(for e.g. `postgresql://user:password@localhost:5432/motum?schema=public`)

Unfourtunately you'll need to manually create empty `.env` files inside of the `cloud-auth` and `cloud-user-registry` folders