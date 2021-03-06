---
path: '/materials/swapi-graphene'
type: 'GitHub'
img: './screenshot.png'
material:
  title: 'swapi-graphene'
  url: 'http://swapi.graphene-python.org'
  github_url: 'https://github.com/graphql-python/swapi-graphene'
  subscribers_count: '7'
  stargazers_count: '155'
  tags: ['']
  subtitle: 'GraphQL Starwars API using Graphene and Django'
  clone_url: 'https://github.com/graphql-python/swapi-graphene.git'
  ssh_url: 'git@github.com:graphql-python/swapi-graphene.git'
  pushed_at: '2018-06-13T06:31:51Z'
  updated_at: '2019-01-05T05:56:04Z'
  author:
    name: 'graphql-python'
    avatar: 'https://avatars3.githubusercontent.com/u/15002022?v=4'
    github_url: 'https://github.com/graphql-python'
  latestRelease:
    tag_name: null
    name: null
    url: null
    created_at: null
---
# GraphQL SWAPI using Graphene 

This is a integration example of [Graphene](http://graphene-python.org) in Django.
[View demo](http://swapi.graphene-python.org/)


## Structure

All the [models](./starwars/models.py) and [fixtures](./starwars/fixtures/) are based in the original [swapi project](https://github.com/phalt/swapi).

The schema (*where all the magic happens*) is in [starwars/schema.py](./starwars/schema.py).
> Look ma, a GraphQL integration with Django models in less than 150 LOC!


## Deploying locally

You can also have your own GraphQL Starwars example running on locally.
Just run the following commands and you'll be all set!

```bash
git clone git@github.com:graphql-python/swapi-graphene.git
cd swapi-graphene

# Install the requirements
pip install -r requirements_base.txt

# Collect static data
python manage.py collectstatic

# Setup the db and load the fixtures
python manage.py migrate
```

Once you have everything done, just run:

```bash
python manage.py runserver
```

Open your browser and visit [localhost:8080](http://localhost:8080/) et voilá!


## Deploying on [Heroku](http://heroku.com)

To get your own GraphQL Starwars example running on Heroku, click the button below:

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/graphql-python/swapi-graphene)

Fill out the form, and you should be cooking with gas in a few seconds.
