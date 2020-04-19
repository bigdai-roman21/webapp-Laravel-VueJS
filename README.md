# vuejs-laravel
VueJS + webpack + semantic-UI + Laravel

- A rapid development framework separated before and after.
- Comes with Laravel's basic account system.
- Front-end single-page web application
- Webpack build front page
- Use babel to support ECMAScript6
- Use Vue's single file component
- Use the latest vue-cli 2.0

## installation

1. Clone code
2. Install background

    ```
        cd backend
        composer install
        // https://laravel.com/docs/5.2
        php artisan key:generate
        php artisan vendor:publish
        php artisan migrate
    ```

3. Configure web server, need to support PHP5.6 or above. For example, the domain name is vuejs-laravel. The server root is configured to the project publicdirectory. ( Be careful not to bebackend/public )
4. Install the front desk

    ```
        cd frontend
        npm install
        
    ```

5. Configure the foreground and background agents. Open frontend/config.js, edit proxyTableto connect to back-end API. Reference: http://vuejs-templates.github.io/webpack/proxy.html

6. Finished

## Development


```
    cd frontend
    npm run dev
```

Then visit http: // localhost: 8080

frontend/srcThe directory contains front-end code. Code changes can be reflected in the browser in real time, and I am puzzled.

backend Inside the directory is the typical Laravel backend codec

## release

```
    cd frontend
    npm run build
```

Then compiled front-end code will appear in publicthe directory. Visit your local web server to browse.

### References

- Laravel: [http://www.laravel.com](http://www.laravel.com)
- VueJS:  [http://www.vuejs.org](http://www.vuejs.org)
- VueJS Templates: [http://vuejs-templates.github.io/webpack/index.html](http://vuejs-templates.github.io/webpack/index.html)
- Webpack: [http://webpack.github.io](http://webpack.github.io)
- Semantic-UI: [http://semantic-ui.cn](http://semantic-ui.cn)

to be continued
