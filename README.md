# Avad.io

## Avadio music

To start the project clone this repository.

## Back-end setup

Create a new virtualenv with python 3.5
Place outside the root project folder.  I place mine in my home directory in an envs/ folder.

```
virtualenv -p python3 --no-site-packages avadioenv
```

cd into the project root folder and use pip to install the necessary packages from the requirements.txt document.

```
cd avadio/

pip install -r .
```

cd into the django project folder 'avadio/' and you can now run the django dev server.

## Front-end setup

run these commands from an additional terminal window.  You will need to run the server and the front-end development server simultaneously.

cd into the folder 'front/' from the django root directory.

Install npm (node) if you do not already have it.

run npm install from the front folder.

```
npm install
```

Once finished you should be able to run the front-end development build server by running the npm run dev command from the front folder.

```
npm run dev
```

Once you have your front-end code working how you like it you can build it.  

```
npm run build
```

This will compile and package up the front-end code into the build/ folder.  It can now be accessed and tested from the main django server.

## Running the servers

Running the django server and accessing the site from localhost:8000 will run the front-end code in the front/build/ folder.

During development you should run the build server listed above in the front-end section.  This will run the front-end code on localhost:8080

Once you've run npm run build the code will compile into front/build/ and be available from the django server on port 8000.  This is what we will deploy.

## Testing

```
npm run test
npm run e2e
```

test: unit tests
e2e: end to end tests for front end display functionality.

Default tests.  Will update as we progress.
