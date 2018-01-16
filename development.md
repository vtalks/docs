# vtalks developer environment

## Requirements

You will need to have installed the following dependencies:

* Docker
* Docker Compose
* Python 3

## Setup the environment

Clone the *deploy* repository:

```bash
git clone git@github.com:vtalks/deploy.git
```

Inside the repository you'll find an `environment.dist.sh` file. 
Copy it to for example `environment.sh` and fill the information 
needed on it.

Once your are finish source it into your shell to have all variables
and aliases loaded:

```bash
source environment.sh
```

## Build containers

### Database

```bash
compose up postgres -d
```

### Web

```bash
compose up web -d
```
