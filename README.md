### Running the application locally for development by Usman

Clone the repository and install dependencies

```git clone https://github.com/usmanjaved156/diabetesFood.vue.git
> cd diabetes-food-database
> npm install
```

Start the backend lambda service and serve the client

```
> npm run start:lambda
> npm run start:vue
```

The user interface will be available at http://localhost:8080/

## Built with

- [Axios](https://github.com/axios/axios) - Querying the database from the client
- [Fuse](http://fusejs.io/) - Fuzzy text search
- [Icons8](https://icons8.com) - Icon/favico
- [Netlify](https://netlify.com) - Hosting the client and the database API
- [Pluralize](https://github.com/blakeembrey/pluralize) - Helping normalize search queries
- [Vue](https://vuejs.org) - User interface
- [webpack-auto-inject-version](https://github.com/radswiat/webpack-auto-inject-version) - Place version at bottom of client
