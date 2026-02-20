Requirements
------------

  - [Docker](https://www.docker.com)
    - [Docker Compose](https://docs.docker.com/compose/)
  - [GNU Make](https://www.gnu.org/software/make/) (optional)

Installation
------------

  1. Clone the repository

         git clone git@github.com:PHLAK/plume-compose.git

  2. Initialize the configuration files

          make init

     or manually run the commands in `Makefile`

  3. Set the environment variables in `.env`

  4. Run `docker compose config` to validate and confirm your configuration

  5. Run `docker compose up -d` to start the containers

Configuration
-------------

Your Plume installation can be configured by adding environment variables to the
`environment.d/plume.env` file. See the [Plume Documentation](https://docs.plume.pub)
for the list of available environment variables and what they do.

> [!IMPORTANT]
> After modifying `environment.d/plume.env` you must restart your containers
> (i.e. `docker compose up -d`) for the changes to apply.
