[![Wase ECS logo banner](http://wase-ecs.com/img/banner.png)](https://wase-ecs.com/)

[![Website badge](https://img.shields.io/website?up_message=online&url=https%3A%2F%2Fwase-ecs.com%2F)](https://wase-ecs.com/)
[![Discord badge](https://img.shields.io/discord/864845724444393472?label=discord)](https://discord.gg/2RBMMxMJ7R)
[![Mit License badge](https://img.shields.io/apm/l/vim-mode)](https://github.com/Wase-ECS/wase-ecs/blob/master/LICENSE)
[![Issues badge](https://img.shields.io/github/issues/Wase-ECS/wase-ecs-website)](https://github.com/Wase-ECS/wase-ecs-website/issues)
![Lines badge](https://img.shields.io/tokei/lines/github/Wase-ECS/wase-ecs-website)
![Stars badge](https://img.shields.io/github/stars/Wase-ECS/wase-ecs-website?style=social)

This repository contains the website source code for the [Wase ECS](https://github.com/Wase-ECS/wase-ecs) repository.

## Requirements
- PHP 8.0 or higher
- Composer
- Symfony
- Yarn
- NPM

## Setting up the website

To run the website on your local environment you will need to create an .env file in the project root and add the following lines to it:
```
APP_ENV=dev
APP_SECRET=
```

After this you will have to run the following commands:
```
composer install
yarn
yarn build
git submodule init
git submodule update
git submodule foreach git pull origin production
```

To start the server you can use `symfony server:start`
