### Installation

1. `mkdir -p data/{sentry,postgres}`
2. `docker-compose run --rm web config generate-secret-key` - Generate a secret key as `SENTRY_SECRET_KEY` in .env.
3. Copy & fill the `.env.dist` to `.env`
4. Copy & fill the `config.yml.dist` to `config.yml`
3. `docker-compose run --rm web upgrade` - Build the database and answer "yes" to create a user account.
4. `docker-compose up -d`
5. Access your instance at `example.com:9000`. Now, create team, project and start monitoring.
