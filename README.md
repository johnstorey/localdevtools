This is just some servers that are usually remote but which I am trying out locally. Currently we have:

- Jenkins 2.0
- Gogs

# Install

Create two directories after you clone the repository:
- gogsrepo
- mysqlrepo

Since I did not bother NOT hard-coding the paths in the docker-compose.yml file (see the double negative!), you'll have to change it to match your host machine directory structure.

Run it.

You'll have Jenkins 2.0 and Gogs. Right now, just install Gogs with the SQL-lite option. Something about Gogs having it's own host resolution code preventing it working with the name resolution inside the private network created by docker-compose. At least that seems the prevalent theory on dicussion boards.

Do not ignore the message on Gogs that says 'follow these instructions to run in Docker.' If you are looking for the IP address of the Gogs container, just run 'docker inspect <container-name>' on your host machine. It will be near the end of the output.


