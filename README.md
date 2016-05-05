This is just some servers that are usually remote but which I am trying out locally. Currently we have:

- Jenkins 2.0
- Gogs

# Install

Create two directories after you clone the repository:
- gogsrepo
- mysqlrepo

Since I did bother NOT hard-coding the paths in the docker-compose.yml file (see the double negative!), you'll have to change it for those repositories.

Run it.

You'll have Jenkins 2.0 and Gogs. Right now, just install Gogs with the SQL-lite option. Something about Gogs having it's own host resolution code preventing it working with the name resolution inside the private network created by docker-compose. At least that seems the prevalent theory on dicussion boards.


