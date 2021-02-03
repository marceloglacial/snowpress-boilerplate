![Heroku](https://pyheroku-badge.herokuapp.com/?app=snowpress-boilerplate)

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
- Local development: <a href='https://www.docker.com/'>Docker</a>

## How to Install

### Local development

1. Make sure `docker` is running
2. Config your `.env` file using `.env.example` as template
3. Open your terminal
4. Run: `composer update` 
5. Run: `npm run dev`
6. Open your local wordpress: [http://localhost:8080](http://localhost:8080)

### Heroku Setup 

1. [Connect your github repository to heroku](https://devcenter.heroku.com/articles/github-integration)
2. Enable `Automatic deploys` on Deploy page
3. Add `JawsDB Maria` on [your add-ons](https://devcenter.heroku.com/articles/managing-add-ons)
4. Add `Heroku Redis` on [your add-ons](https://devcenter.heroku.com/articles/managing-add-ons)
5. Add `heroku/php` on your buildpacks (settings page)
6. Add your `.env` variables on [settings page](https://devcenter.heroku.com/articles/config-vars)
7. Configure your <a href='https://uptimerobot.com/'>Uptime Robot</a> to 20 min to avoid dyno resets
8. Open your app

## IMPORTANT

Heroku [ephemeral filesystem](https://help.heroku.com/K1PPS2WM/why-are-my-file-uploads-missing-deleted) is not suitable for persistent storage of data/files. That's why **Cloudinary Plugin is a mandatory setup**.

Make sure to select `Cloudinary Only` on Cloudinary > Media settings > Sync > Storage.
