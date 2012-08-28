# What is MongoTor ?

(MONGO + TORnado) is an asynchronous toolkit for accessing mongo with tornado.

## Features

* ORM like to map documents and fields
* Advanced connection management (replica sets, slave okay)
* Automatic reconnection
* Connection pooling
* Support for running database commands (find, find_one, count, sum. etc...)

## Why not pymongo ?

[PyMongo](http://api.mongodb.org/python/current/) is a recommended way to work with MongoDB in python, but isn't asynchronous and not running inside de tornado's ioloop. If you use pymongo you won't take the advantages of tornado.

## Whi not asyncmongo ?

[AsyncMongo](https://github.com/bitly/asyncmongo) is asynchronous library for accessing mongo with tornado.ioloop, but don't implement replica set, don't have an ORM, I don't like her connection pooling, is deficitary, and i don't trust in your tests. 

Besides, this project is not walking very well, or better, very fast. Exist a lot of issues and pull requests that aren't looked.

I am very thankful to asyncmongo, i worked with he in some projects and he's been served as inspiration, but now, I am very excited to write my own library, more flexible, fast, secure and that will walking faster.