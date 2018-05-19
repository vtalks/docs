# vtalks developer environment

## Requirements

You will need to have installed the following dependencies:

* Docker & Docker Compose
* Python 3+

## Get the source code

Clone the current needed repositories:

```bash
mkdir vtalks
cd vtalks
git clone git@github.com:vtalks/branding.git
git clone git@github.com:vtalks/deploy.git
git clone git@github.com:vtalks/docs.git
git clone git@github.com:vtalks/facebook_worker.git
git clone git@github.com:vtalks/linkedin_worker.git
git clone git@github.com:vtalks/twitter_worker.git
git clone git@github.com:vtalks/updater_worker.git
git clone git@github.com:vtalks/vtalks.net.git
```

In this guide, if it is not specified the working directory will be the 
`vtalks` directory created where all other repos reside.

## Setup the environment

Inside the `deploy` repository you'll find an `environment.dist.sh` file. 
Copy it to for example `environment.sh` and fill the information 
needed on it.

Once you finish, source it inside your current shell to have all environment 
variables and aliases loaded:

```bash
source environment.sh
```

## Build containers

All project is deployed using docker containers. Follow this instructions to 
build, deploy and run them:

### Database

Inside `deploy` folder repository, build and run the database container with:

```bash
compose up -d postgres
```

##### Import and Export database data

To import the database from a backup execute:

```bash
compose exec postgres /restoredb.sh
```

To export the database execute:

```bash
compose exec postgres /dumpdb.sh
```

##### Configuration & Environment variables

> [ISSUE-deploy/2](https://github.com/vtalks/deploy/issues/2):
> Environment variables to configure the database.

### Web

Inside `deploy` folder repository, build the container image with:

```bash
compose up -d web
```

And copy static files:

```bash
manage collectstatic
```

#### Execute tests suite

Inside `vtalks.net` folder repository, execute the tests suite into a  container:

```bash
make test
```

Generate coverage report and send it to coveralls.io:

```bash
make cover
```

#### Build and Publish docker image

Inside `deploy` folder repository, build the container image with:

```bash
make docker-build
```

And publish the built container image with:

```bash
make docker-publish
```

### Ningx

```bash
compose up -d nginx
```
