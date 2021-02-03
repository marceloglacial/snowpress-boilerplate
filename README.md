![Heroku](https://pyheroku-badge.herokuapp.com/?app=serlares-2021)

# SnowPress Boilerplate

A WordPress installation optimized for Docker and Heroku

## Live Demo

- <a href="https://serlares-2021.herokuapp.com/">Heroku</a>
- ## Stack and Features

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

NOTE: Make sure `docker` is running

```
composer update
npm run dev
```

## Heroku Setup 
1. Add your `.env` variables 
2. Add `JawsDB Maria` on your add-ons
3. Add `Heroku Redis` on your add-ons
4. Add `heroku/php` on your buildpacks
