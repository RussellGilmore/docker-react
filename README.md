# React Dockerized
This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## About
This is an example I have built on showing how to orchestrate the building of a React pipeline with a solid React local development environment with tests. It uses Travis CI to build and deploys to AWS ELastic Beanstalk.  

## Running
```sh
# Easy
~ docker-compose up
Creating network "docker-react_default" with the default driver
Creating docker-react_web_1   ... done
Creating docker-react_tests_1 ... done
Attaching to docker-react_tests_1, docker-react_web_1
tests_1  |
tests_1  | > frontend@0.1.0 test /app
tests_1  | > react-scripts test
tests_1  |
web_1    |
web_1    | > frontend@0.1.0 start /app
web_1    | > react-scripts start
web_1    |
web_1    | ℹ ｢wds｣: Project is running at http://172.19.0.3/
web_1    | ℹ ｢wds｣: webpack output is served from
web_1    | ℹ ｢wds｣: Content not from webpack is served from /app/public
web_1    | ℹ ｢wds｣: 404s will fallback to /
web_1    | Starting the development server...
web_1    |
tests_1  | PASS src/App.test.js
tests_1  |   ✓ renders without crashing (46ms)
tests_1  |
tests_1  | Test Suites: 1 passed, 1 total
tests_1  | Tests:       1 passed, 1 total
tests_1  | Snapshots:   0 total
tests_1  | Time:        3.621s
tests_1  | Ran all test suites.
tests_1  |
web_1    | Compiled successfully!
web_1    |
web_1    | You can now view frontend in the browser.
web_1    |
web_1    |   Local:            http://localhost:3000
web_1    |   On Your Network:  http://172.19.0.3:3000
web_1    |
web_1    | Note that the development build is not optimized.
web_1    | To create a production build, use yarn build.
web_1    |
```
You should then be able to hit your app at the following [localhost](localhost:3000).

Run `docker-compose down` to teardown.