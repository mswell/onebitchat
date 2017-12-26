![rails](https://img.shields.io/docker/automated/jrottenberg/ffmpeg.svg)

# Onebitchat

This application is a Slack clone, created on [OneBitCode](http://onebitcode.com/) BootCamp <3

Technologies used in this app:

- [Rails](http://rubyonrails.org/)
- [Docker](https://docs.docker.com/)
- [PostgreSQL](https://www.postgresql.org/)
- [Materialize](http://materializecss.com/)
- [CoffeeScript](http://coffeescript.org/)

## Dependencies

- [Docker](https://docs.docker.com/)
- [Docker-Compose](https://docs.docker.com/compose/)

## Initial setup

At first, you need to setup some configurations after clonning the repo to your local machine.

### Setup in your machine

 ```sh
 docker-compose up --build
 docker-compose run --rm website bundle install
 docker-compose run --rm website bundle exec rake db:create db:migrate
 docker-compose up 
 ```
Happy fun :)

## Test
```sh
  docker-compose run --rm website bundle exec rspec
```

## Contributing to this project

 **1. Fork the project**

 **2. Clone the fork to your machine**

 ```sh
 git clone git@github.com:YOUR-USERNAME/YOUR-FORKED-REPO.git
 ```

 **3. Set the remote upstream from original repository**

 ```sh

 cd into/cloned/fork-repo
 git remote add upstream https://github.com/mswell/onebitcode_exchange.git
 git fetch upstream
 ```
 **4. Submitting Pull Requests:**

 * work on your local branch and submit it to your fork master.

 * Create a PR from your branch to the original repository.


 **5. Syncing a fork**

 [Follow the steps in this link](https://help.github.com/articles/syncing-a-fork/)


<h6 align="center">
	<a href="https://goo.gl/EHhrcC">MIT</a>
	©
	Wellington Moraes
</h6>
