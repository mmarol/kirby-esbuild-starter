## esbuild Kirby Starter
- kirby installed through composer for easy updating
- esbuild and PostCSS for JS and CSS asset compiling.
- BrowserSync for live reloading

## Setup
- `composer install` to make sure kirby is installed
- `npm install` to load all dependencies
- `npm run watch` for development
- `npm run build` for production
- `composer update getkirby/cms` to update the Kirby version

## Notes
- No hot module replacement
- Targets latest CSS and JS specifications. Can change that in the scripts.
- `/package.json` has scripts for watching and building
- Make sure you change the local dev URL to proxy in the `/package.json` scripts
- Add PostCSS plugins to `/postcss.config.js`. Currently doesn't use any plugins.
- `rsync` script is a placeholder, haven't figured it out yet
- Includes a bunch of Kirby blueprints and templates

## To-do
- [ ] figure out rsync
- [ ] figure out esbuild targets to compile for older browsers
- [ ] see if PostCSS is actually necessary to include
- [ ] see if `esbuild serve` can be used instead of browsersync
