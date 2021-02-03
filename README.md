![Heroku](https://snowpress-boilerplate.herokuapp.com/)

# SnowPress Boilerplate

A WordPress installation optimized for Docker and Heroku

## Live Demo

- <a href="https://snowpress-boilerplate.herokuapp.com/">Heroku</a>

## Stack and Features

- CMS: <a href="https://wordpress.org/">WordPress</a>
- PHP dependency Manager: <a href="http://getcomposer.org/">Composer</a>
- Project structure: <a href="https://roots.io/bedrock/">BedRock</a>
- Deployment: <a href="https://github.com/PhilippHeuer/wordpress-heroku">WordPress on Heroku</a>
- Heroku Keep Alive: <a href='https://uptimerobot.com/'>Uptime Robot</a>
- Image CDN: <a href="https://cloudinary.com/">Cloudinary</a>
- Site Builder: <a href="https://github.com/marceloglacial/snow-blocks">Snow Blocks</a>
- Local development: <a href='https://www.docker.com/'>Docker</a>

## How to Install

1. Config your `.env` file using `.env.example` as model
2. Run composer to install dependencies: `composer update`
3. Set Wordpress permalinks to `Post Name`

## Local development

1. Make sure `docker` is running
2. Open your terminal
3. Run: `composer update` 
4. Run: `npm run dev`
5. Open your local wordpress: [http://localhost:8080](http://localhost:8080)

## Heroku Setup 

1. [Connect your github repository to heroku](https://devcenter.heroku.com/articles/github-integration)
2. Add `JawsDB Maria` on [your add-ons](https://devcenter.heroku.com/articles/managing-add-ons)
3. Add `Heroku Redis` on [your add-ons](https://devcenter.heroku.com/articles/managing-add-ons)
4. Add `heroku/php` on your buildpacks (settings page)
5. Add your `.env` variables on [settings page](https://devcenter.heroku.com/articles/config-vars)
