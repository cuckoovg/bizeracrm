BizeraCRM 1.2.1 Tim Dev

# Support Terms

1 - The support on Bizera only applies to the information provided by the users while creating an issue. This means we won't either do the installation on your server or check an issue on your server. You're therefore invited not to post your server information while creating an issue. We'll use your explanations to reproduce your issue and therefore to solve it.

# Troubleshooting
Here we list the knowns issues and the way around. Not everyone is likely to face these issues as it depends on the used enviroment.

- CSRF error After Installation
Chances are when you make your installation, you'll have your website URL changed. Unfortunately, if the domain has to change, it must be clearly described on the .env file. 

- Error After Database Details (using `php artisan serve`)
If you're serving the project using `php artisan serve`, after setting up the database credentails and having them validated, you migth stop on an infinite
loading page. 

This is caused because during the database setup, the ".env" is updated which cause Laravel to restart the development server and therefore invalidate your session. The way around, is just to refresh the page and you'll end up on the application details section.

## Contribution Guidelines
Do you plan to contribute? That's awesome. We don't have that much developer on it, so we're open to any type of contributions. If you're a developper, you'll start by forking the project and deploying that locally for further tests. Typically, you'll need to build the project (Vue.js) in watch mode. You'll then start by making sure the .env value "NS_ENV" is set to "dev". From there, you can run the following command :

**To install Node.js dependencies**
```
npm install
```

**To watch the Vue compoment changes (Vue.js)**
```
npm run dev
```

**To watch the project changes (TailwindCSS)**
```
npm run css-watch
```

**To build the project for production, you'll need to only run that command:**
This will build the JavaScript file and CSS files.

```
npm run prod
```
