# vtalks developer environment

## Requirements

You will need to have installed the following dependencies:

* Docker & Docker Compose
* Python 3+

## Setup the environment

Clone repositories:

```bash
mkdir vtalks
cd vtalks
git clone git@github.com:vtalks/branding.git
git clone git@github.com:vtalks/deploy.git
git clone git@github.com:vtalks/docs.git
git clone git@github.com:vtalks/vtalks.net.git
```

Inside the repository you'll find an `environment.dist.sh` file. 
Copy it to for example `environment.sh` and fill the information 
needed on it.

Once you finish, source it inside your current shell to have all variables
and aliases loaded:

```bash
source environment.sh
```

## Build containers

### Database

```bash
compose up -d postgres
```

### Web

```bash
compose up -d web
```

### Ningx

```bash
compose -up -d nginx
```
