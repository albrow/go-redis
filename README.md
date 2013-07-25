go-redis
========

A fork of the tgcl redis library. Supports unix sockets, most/all redis commands, and has automatic pooling.

The original repository on which this is based lives at http://godoc.org/code.google.com/p/tcgl/redis.
The only difference between the official branch and this one is that this one supports unix sockets.
Much thanks to Frank Mueller, the maintainer of [tcgl](https://code.google.com/p/tcgl/).

How to Use
==========

#### To install:

    go get github.com/stephenalexbrowne/go-redis
    
Or add `github.com/stephenalexbrowne/go-redis` to your import list.

#### To connect using unix sockets:

(Assuming you have configured redis to use a unix socket at /tmp/redis.sock)

    db := Connect(Configuration{
		UseSockets: true,
		Address:    "/tmp/redis.sock",
	}) 

#### More examples

Check the [Official branch](http://godoc.org/code.google.com/p/tcgl/redis) for the full documentation.

You can also look at the [redis_test.go](https://github.com/stephenalexbrowne/go-redis/blob/master/redis_test.go)
file for usage examples. I may add some more stuff here in the future.

