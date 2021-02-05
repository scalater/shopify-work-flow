# Shopify workflow example
This repository is only an example of the basic workflow and it is based on `themekit`.

#My personal vision
Each theme you create in the store is like individual environments, from this point of view we can create them as needed to take advantage of collaborative workflows.

##Requirements
This workflow need **themekit**

##Before Start
- Install `themekit`
    - https://shopify.dev/tools/theme-kit/getting-started
- Configure the `config.yml` using `config.example.yml`
- Run `npm i` to get dev dependencies

##Directory Structure
- sass --> source of sass
- theme --> theme directory mirror from the shopify environment

##First steps
- First clone the repo
- Create develop environment duplicating the production theme
- Configure the `config.yml` to match the develop theme
- Download it using the npm command `npm run downlaod`
- Add&commit all new files under the theme folder to git
- Done you have your develop environment tracked and ready

##Workflow
- To start work you need to run 2 commands from the project directory
    - `gulp` --> watch sass changes and compile to css and sync to `theme/assets/theme.css.liquid`
    - `npm watch` --> watch any change inside the `theme` folder and sync with the develop environment
- To open the theme preview run
    - `npm run open`

## Next challenge
- Connect with a CD services


