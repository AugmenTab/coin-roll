# Coin Roll

This application is a proof-of-concept for a customizable cryptocurrency dashboard. It allows the user to search a database of cryptocurrencies and create their own watchlist of those that interest them. Their watchlist provides current financial and portfolio information on the cryptocurrencies in their watchlist. They can also insert a transaction record, a purchase or a sell, and see a summary of their portfolio that includes data like their current investment's value and the profit they've made so far, on both a per-cryptocurrency and overall scale.

## Implementations

* [Coin Roll Python](/coinroll-python): The first implementation of this project was written in [Python 3](https://www.python.org/), using [FastAPI](https://fastapi.tiangolo.com/) with [Uvicorn](https://www.uvicorn.org/), [Asyncio](https://docs.python.org/3/library/asyncio.html), [Celery](https://docs.celeryproject.org/en/stable/index.html) with [RabbitMQ](https://www.rabbitmq.com/), and [Pydantic](https://pydantic-docs.helpmanual.io/). The database was [MongoDB](https://www.mongodb.com/) using [MongoEngine](http://mongoengine.org/). Testing was done with [Pytest](https://docs.pytest.org/en/6.2.x/).
* [Coin Roll Haskell](/coinroll-haskell): Currently still in the planning phase, the [Haskell](https://www.haskell.org/) implementation will be built on either [Servant](https://docs.servant.dev/en/stable/), [WAI](https://hackage.haskell.org/package/wai), or [Yesod](https://www.yesodweb.com/). The database will be either [MongoDB](https://www.mongodb.com/) or [PostgreSQL](https://www.postgresql.org/). Testing will likely be done with [QuickCheck](https://hackage.haskell.org/package/QuickCheck).

## Future Planned Implementations

The following is a list of Coin Roll implementations I plan to write in the future, in no particular order.

* Coin Roll [Erlang](https://www.erlang.org/)
* Coin Roll [Clojure](https://clojure.org/) w/ [Datomic](https://www.datomic.com/) database
* Coin Roll [Rust](https://www.rust-lang.org/)
* Coin Roll Prolog, using either [GNU Prolog](http://www.gprolog.org/), [SWI-Prolog](https://www.swi-prolog.org/), or [YAP](https://www.dcc.fc.up.pt/~vsc/yap/).
* Coin Roll [Mercury](https://mercurylang.org/)
