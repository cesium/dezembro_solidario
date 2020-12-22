[contributing]: CONTRIBUTING.md
[code_of_conduct]: CODE_OF_CONDUCT.md
[license]: LICENSE.txt
[cesium]: https://cesium.di.uminho.pt
[cesium-logo]: https://raw.githubusercontent.com/cesium/dezembro_solidario/ne/readme/.github/cesium_preto.png

<a href="https://dezembrosolidario.cesium.di.uminho.pt" target="_blank">
  <img align="right" src="img/sticker.png" alt="Dezembro Solidário" width="250">
</a>

# :christmas_tree: Dezembro Solidário

[![Netlify Status](https://api.netlify.com/api/v1/badges/eccde42a-3f33-470d-a3e0-d21872e8899a/deploy-status)](https://app.netlify.com/sites/dezembro-solidario/deploys)

O Dezembro Solidário é um projeto de cariz social, que tem como objetivo trazer
uma maior celebração da época natalícia à [Universidade do
Minho](https://www.uminho.pt/PT) através de incentivos à união da comunidade
académica, espalhando decorações e unindo as nossas associações de estudantes
num espírito de solidariedade e partilha, já que no final do mês todos os bens
recolhidos durante a atividade serão oferecidos a uma instituição social de
ajuda aos mais necessitados.

## :rocket: Getting Started

These instructions will get you a copy of the project up and running on your
local machine for development and testing purposes.

### :inbox_tray: Prerequisites

The following software is required to be installed on your system:

- [ruby](https://www.ruby-lang.org/en/downloads/)

Install all dependencies using `bundle install`.

### :hammer: Development

Starting the development server at <http://localhost:4000>.

```
rake develop
```

This is the default task, so you can run just `rake`.

### :package: Deployment

Bundling the website into static files for production.

```
rake build
```

### :whale: Docker

You can also use a docker container if you prefer.

Setup the container.

```
docker-compose up -d
```

Start the development server and go to http://localhost:4000.

```
docker-compose start
```

Stop the development server.

```
docker-compose stop
```


## :handshake: Contributing

Please read [CONTRIBUTING][contributing] and [CODE_OF_CONDUCT][code_of_conduct]
for details on our code of conduct and the process for submitting pull requests
to us.

## :memo: License

This project is licensed under the MIT License - see the [LICENSE][license] file
for details.

## :sparkles: About

This website was developed with :heart: by [CeSIUM][cesium].

[![CeSIUM][cesium-logo]][cesium]


