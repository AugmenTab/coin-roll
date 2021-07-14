# Coin Roll

This application is a proof-of-concept for a customizable cryptocurrency dashboard. It allows the user to search a database of cryptocurrencies and create their own watchlist of those that interest them. Their watchlist provides current financial and portfolio information on the cryptocurrencies in their watchlist. They can also insert a transaction record, a purchase or a sell, and see a summary of their portfolio that includes data like their current investment's value and the profit they've made so far, on both a per-cryptocurrency and overall scale.

## Implementations

* [Coin Roll Python](coinroll-python/README.md): The first implementation of this project was written in [Python 3](https://www.python.org/), using [FastAPI](https://fastapi.tiangolo.com/) with [Uvicorn](https://www.uvicorn.org/), [Asyncio](https://docs.python.org/3/library/asyncio.html), [Celery](https://docs.celeryproject.org/en/stable/index.html) with [RabbitMQ](https://www.rabbitmq.com/), and [Pydantic](https://pydantic-docs.helpmanual.io/). The database was [MongoDB](https://www.mongodb.com/) using [MongoEngine](http://mongoengine.org/). Testing was done with [Pytest](https://docs.pytest.org/en/6.2.x/).
* [Coin Roll Haskell](https://github.com/AugmenTab/coinroll-haskell): Currently still in the planning phase, the [Haskell](https://www.haskell.org/) implementation will be built on either [Servant](https://docs.servant.dev/en/stable/), [WAI](https://hackage.haskell.org/package/wai), or [Yesod](https://www.yesodweb.com/). The database will be either [MongoDB](https://www.mongodb.com/) or [PostgreSQL](https://www.postgresql.org/). Testing will likely be done with [QuickCheck](https://hackage.haskell.org/package/QuickCheck).

## Common Technology Used

Below is a list of all the important technology used in the production of all implementations of Coin Roll.

### Development Environment

* [Docker](https://www.docker.com/): Each app lives in Docker containers managed using the Docker Desktop app for Windows.
* [Docker Compose](https://docs.docker.com/compose/): This is used to set up a virtual development environment to host all of the servers the applications utilize in order to function.

### Code Quality &amp; Continuous Integration

* [CircleCI](https://circleci.com/): This performs unit tests and ensures their passing after any commits are pushed to GitHub.
* [githooks](https://git-scm.com/docs/githooks): A number of fairly simple pre-commit githooks run unit tests, and block the commit if the tests fail.

### External Services

* [CoinMarketCap API](https://coinmarketcap.com/api/): The API I chose to use for providing cryptocurrency information. The Basic level is free, and permits 333 "credits" (typically a call with less than 100 coins on it will cost a single credit) per day, and up to 10,000 "credits" per month. It has a much more limited suite of information available, but for this proof of concept, it is more than sufficient.

## Future Planned Implementations

The following is a list of Coin Roll implementations I plan to write in the future, in no particular order.

* Coin Roll [Erlang](https://www.erlang.org/)
* Coin Roll [Clojure](https://clojure.org/) w/ [Datomic](https://www.datomic.com/) database
* Coin Roll [Rust](https://www.rust-lang.org/)
* Coin Roll Prolog, using either [GNU Prolog](http://www.gprolog.org/), [SWI-Prolog](https://www.swi-prolog.org/), or [YAP](https://www.dcc.fc.up.pt/~vsc/yap/).
* Coin Roll [Mercury](https://mercurylang.org/)
