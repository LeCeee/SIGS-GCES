# SIGS - Sistema Inteligente de Gestão de Salas


![screen shot 2018-10-08 at 18 43 00](https://user-images.githubusercontent.com/18387694/46635580-54b54c00-cb2b-11e8-8e16-b3d2e41de814.png)


[![BuildStatus](https://travis-ci.org/GCES-2018-2/SIGS-GCES.svg?branch=develop)](https://travis-ci.org/GCES-2018-2/SIGS-GCES)
[![Maintainability](https://api.codeclimate.com/v1/badges/0fbe067cc9bb564ce2bf/maintainability)](https://codeclimate.com/github/GCES-2018-2/SIGS-GCES/maintainability)
[![Test Coverage](https://api.codeclimate.com/v1/badges/0fbe067cc9bb564ce2bf/test_coverage)](https://codeclimate.com/github/GCES-2018-2/SIGS-GCES/test_coverage)
[![Ruby](https://img.shields.io/badge/ruby-2.5.1-blue.svg)](https://www.ruby-lang.org)
[![Rails](https://img.shields.io/badge/rails-5.0.2-blue.svg)](http://rubyonrails.org/)
[![MIT License](https://img.shields.io/badge/license-MIT%20License-blue.svg)](https://opensource.org/licenses/MIT)

SIGS is a Ruby on Rails website project design for UnB (University of Brasília). The project aims to facilitate and automate the process of allocation of university rooms by city officials, coordinators and other stakeholders. For more informations see the [The Wiki Project](https://github.com/fga-gpp-mds/2017.1-SIGS/wiki).

## Features

To see the features of the project [Click Here](https://github.com/fga-gpp-mds/2017.1-SIGS/releases).

## Heroku Deploy

To View Application Deploy [Click Here](https://sigsunb.herokuapp.com)

## License

To see the license of the project [Click Here](https://github.com/fga-gpp-mds/2017.1-SIGS/blob/master/LICENSE)

## Getting Started

There are 2 ways to set up your environment. You can use Docker to simulate isolate containers that has only the software dependencies, or you can run a virtual machine and simulate a whole system using Vagrant. To each case, you can follow the instructions below.

### Set up using Docker

* Install Docker

  - [Download docker](https://docs.docker.com/engine/installation/)

* Install Docker Compose

  - [Download docker-compose](https://docs.docker.com/compose/install/)

* Build the container image

      $ docker-compose build

* Or download it from [DockerHub](https://hub.docker.com/r/projetosigs/sigs-gces/)

* Run the container

      $ docker-compose up -d

* Set up the Database

  To create the database, run the migration and populate it with fictional data

      $ docker-compose run web rails db:create db:migrate db:seed

* Open the internet browser in http://localhost:3000/.


### Set up using Vagrant
* Install the virtual machine software [VirtualBox](https://www.virtualbox.org).

      $ sudo apt-get install virtualbox

* Install the virtual environment [Vagrant](https://www.vagrantup.com).

      $ sudo apt-get install vagrant

* Clone the project Repository.

      $ git clone https://github.com/fga-gpp-mds/2017.1-SIGS.git

* In the folder of project, rise the virtual environment.

      $ vagrant up --provision

* Run the virtual environment.

      $ vagrant ssh

* Get in the folder of project on [Vagrant](https://www.vagrantup.com).

      $ cd vagrant/SIGS

* Install all the gems used in the project.

      $ bundle install

* Create and populate all the tables of the [MySql](https://www.mysql.com) Database.

      $ rails db:create db:migrate db:seed

* Run the Rails server project on [Vagrant](https://www.vagrantup.com).

      $ rails s -b 192.168.2.15

* Open the internet browser in http://192.168.2.15:3000.


### Using the application

* Login with the desired user.

      DEG User
      e-mail: "deg@unb.br"
      password: "123456"

      Coordinator User
      e-mail: "coordenador@unb.br"
      password: "123456"

      Administrative Assistant
      e-mail: "adm@unb.br"
      password: "123456"

For more install and configurate informations, access the [Tutorial](https://github.com/fga-gpp-mds/2017.1-SIGS/wiki/Comandos-de-Instala%C3%A7%C3%A3o-do-Ambiente).
