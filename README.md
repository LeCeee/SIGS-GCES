# SIGS - Sistema Inteligente de Gestão de Salas

<p align="center"><img width="300" src="https://raw.githubusercontent.com/wiki/fga-gpp-mds/2017.1-SIGS/images/logo/cerebro_black.png"></p>

[![BuildStatus](https://travis-ci.org/fga-gpp-mds/2017.1-SIGS.svg?branch=master)](https://travis-ci.org/fga-gpp-mds/2017.1-SIGS)
![Coverage Status](https://coveralls.io/repos/github/fga-gpp-mds/2017.1-SIGS/badge.svg?branch=development)
[![Ruby](https://img.shields.io/badge/ruby-2.3.1-blue.svg)](https://www.ruby-lang.org)
[![Rails](https://img.shields.io/badge/rails-5.0.2-blue.svg)](http://rubyonrails.org/)
[![MIT License](https://img.shields.io/badge/license-MIT%20License-blue.svg)](https://opensource.org/licenses/MIT)

SIGS is a Ruby on Rails website project design for UnB (University of Brasília). The project aims to facilitate and automate the process of allocation of university rooms by city officials, coordinators and other stakeholders. For more informations see the [The Wiki Project](https://github.com/fga-gpp-mds/2017.1-SIGS/wiki).

## Features

To see the features of the project [Click Here](https://github.com/fga-gpp-mds/2017.1-SIGS/releases).

## Heroku Deploy

To View Application Deploy [Click Here](https://sigs-unb.herokuapp.com)

## License

To see the license of the project [Click Here](https://github.com/fga-gpp-mds/2017.1-SIGS/blob/master/LICENSE)

## Getting Started

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

* Login with the DEG user or the Coordinator user.

      DEG User
      e-mail: "wallacy@unb.br"
      password: "123456"

      Coordinator User
      e-mail: "caio@unb.br"
      password: "123456"

For more install and configurate informations, access the [Tutorial](https://github.com/fga-gpp-mds/2017.1-SIGS/wiki/Comandos-de-Instala%C3%A7%C3%A3o-do-Ambiente).
