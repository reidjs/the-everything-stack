# Development
### Running from docker-compose from nginx-proxy directory
Anytime you change the code make sure to run  
`docker-compose build`  
To start all the services run  
`docker-compose up -d`
To stop all the services run  
`docker-compose down`

### Running individual Dockerfiles
cd into react-next  
`docker build -t reidjs/next-web-app .`  
`docker run -p 49161:3000 -d reidjs/next-web-app`  

cd into vue-vuex  
*note: had to remove fsevents to get this working*  
`docker build -t reidjs/vue-vuex .`  
`docker run -p 49162:3001 -d reidjs/vue-vuex`  

# The Everything Stack
The Everything Stack is a rube-goldberg-esque static website that runs on as many modern technologies as possible.  
In the spirit of https://github.com/EnterpriseQualityCoding/FizzBuzzEnterpriseEdition the goal is to perform _simple tasks_ in the most convoluted method possible. This is an art project and not intended for serious production uses. 

1. React w/ Next
https://github.com/react-next-boilerplate/react-next-boilerplate

2. Vue w/ Vuex
https://github.com/chrisvfritz/vue-enterprise-boilerplate

# Ideas
*Yes:* 
- it clear from the frontend what technologies are being used and why.
- Demo technologies in the right way (e.g., using react to serve a reactive form, not 'hello world')
- Use docker and orchestration 

*No:*
- it does the same thing in 30 different ways. 

*Follow through:*
- Use microservices:
https://blog.logrocket.com/methods-for-microservice-communication/
- A bunch of docker containers all chatting together
https://docker-curriculum.com/
- Run on an EC2 instance

- An online game
- A blog
- A message board
- A pastebin
- Streaming analytics (kafka, spark, cassandra)
- An ethereum dapp 
- A restful API (JAVA AND SPRING BOOT)

# The front page
### Short term goal:  
Link the different containers in a *index* link page.

### Long term goal:  
At its core, visitors should be able to: 
- Create an account
    - recaptcha to prevent spam
- Log in 
- Authenticated users can post 
- Post links, pictures, questions, comments
- Upvote other people's links
- All comments must be related to incorporating new technologies into the site

# List of Tech
https://awesomestacks.dev/

Web Frameworks
- React
    - Gatsby
    - Next
    - Jest
- Svelte
    - Sapper
- Angular
- jQuery
- Vue
    - Nuxt
- Django
- Flask
- Ruby on Rails

Testing Frameworks
- Jest

CI/CD
- Jenkins
- TravisCI
- CircleCI

Analytics
- Matomo
- Google Analytics

Webserver (NOTE: Currently runs on github pages, but a hosted webserver is on the roadmap)
- Express
- NGINX
- Apache



