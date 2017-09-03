# pyapi
docker-compose service using python API and MongoDB

Instructions:
Configure environment variables in 'docker-compose.yml'.

It is advised to use the newest available container versions of zfllj/smplrst and zfllj/mymongo to ensure smooth operation but can be modified as you see fit.

MONGODB_HOST should be the name of your MongoDB container which defaults to 'mongo' in the initial config so there is no reason to change this unless you have good reason.

API_KEY should be set to your API key for the cat API which can be acquired for free [here](http://thecatapi.com/api-key-registration.html)

A 'pythian' bridge network is created and used for container communication and service discovery/DNS. This can be whatever you wish or left out entirely which will cause docker-compose to create an arbitrary default bridge network at run time.

See docker-compose file [reference](https://docs.docker.com/compose/compose-file/) for instructions to customuize your deployment further.
