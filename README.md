## SENTRY Docker-compose 

1. Set environment in .dockerenv.example (only SENTRY_SECRET_KEY can be changed)
2. RUN `mv .dockerenv.example .dockerenv`
3. Run `docker-compose up -d`
4. Run `docker-compose exec sentry sentry upgrade` to setup database and create admin user
5. Run `docker-compose restart sentry`
6. Sentry is now running on public port `9000`
