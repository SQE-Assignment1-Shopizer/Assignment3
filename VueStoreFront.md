## Vue Store Front

### Introduction
Vue Storefront is a standalone Progressive Web Application solution for web stores that can drastically enhance the shopping experience. Moreover, thanks to the ability to connect to an array of eCommerce backend solutions like Magento, Prestashop or Shopware through their respective API, it can be used by any store.  It can also serve as a great code base for developers who build front-end for eCommerce stores. 

### Installation
 To set Up VueStoreFront on your local environment you must have to fulfill the following system requirements.
 
 #### Prerequisites
 
>* NodeJs v14 or latest version This includes a version manager, package manager, and Visual Studio Code. The Node Package Manager (npm) is used to install Vue.js.
>* Vue.js framework
>* Express.js for Server API
>* Elastic Search
>* Docker
>* Vendure server running in localhost for GraphQL API or https://demo.vendure.io/shop-api
>* Set up auth options in Vendure server (This functionality is available for those who scaffold a local instance of Vendure)

### Tools
>* Vue CLI
   Vue CLI is a toolkit for working with Vue in your terminal / command line. It enables you to quickly scaffold a new project (vue create), prototype new ideas (vue serve), or manage projects using a graphical user interface (vue ui).
>* Vue.js DevTools (to view component structiures and theircurrent state)
>* Vetur extension (speeds up developement)
>* add PWA plugin to Vuestore Front after installing Vue CLI
>>* Requirements for PWA
>>>* A JavaScript service worker (to allow the site to load offline and store data locally)
>>>* A valid JSON manifest of the app’s info, with the correct info filled in
>>>* A set of properly named icons, at multiple sizes
>>>* A secure, HTTPS connection
>* Vue Store Front only supports one CI/CD tool which is Githiub Actions


### MicroServices Architecture
Vue Store Front has microservices architecture breaking it into multiple modules. Each module has its own specific responsibilities but communicates with others to form a unified system
![vue](https://user-images.githubusercontent.com/82566358/205505058-2a1e2824-1a1b-4205-ae26-733445ae0c5f.png)

Micro Servicing and Modularity afftes the non functional requirements greatly

>* ##### Reliability
         Micro Services and modularity increases reliability. Any bug in any module (e.g. memory leak) will not  bring down the entire function.
>* ##### Maintainability
         The adoption of new technologies becomes easier Because changes to frameworks or languages will not affect the entire application.Each Update will not require the delpoyment of the entire application.Moreover each service is relatively small and so is easier to understand and change

>* ##### Scalability
         Modular applications are easy to scale when various modules have incompatible resource requirements, continuous deployment is easy.

>* ##### Testability
         Since the services are smaller, they are faster to test

>* ##### Fault Tolerance
         Improved fault isolation. For example, if there is a memory leak in one service then only that service will be affected. The other services will continue to handle requests. In comparison, one misbehaving component of a monolithic architecture can bring down the entire system.

#### Nuxt.js
     Most integrations in Vue Storefront ask you to register a Nuxt.js plugin or module in the nuxt.config.js file. These extend the Application context and add special handlers that allow you to make API calls to the Server Middleware.Composables use the exact mechanism to communicate with their corresponding platforms when you call their methods.
#### Server Middleware
    In Vue Storefront, there is a "proxy" between them called Server Middleware. Server Middleware is an Express.js server that exposes API endpoints defined in the extensions registered in the middleware.config.js file.
   

#### Sevice Providers
     Server Middleware can communicate with various service providers as long as they expose an API. It can use industry-standard libraries like axios or Apollo or platform-specific JavaScript SDKs.

##### DataFlow
      In Vue Storefront, three applications exchange the data:
>* Nuxt.js application - requests data from the Server Middleware when specific methods in the Application context or Composables are called.
>* Server Middleware - accepts requests from the Nuxt.js application, converts them, and sends them to the given platform in the proper format and communication technology.
>* Service providers - expose API endpoints to fetch, add and remove data.
 
 
 ![middleware](https://user-images.githubusercontent.com/82566358/205515180-f6099caa-43a1-44bb-ae36-879ed157a319.png)
 
 
 ### Memory Consumption
 The microservice architecture replaces N monolithic application instances with NxM services instances. If each service runs in its own JVM (or equivalent), which is usually necessary to isolate the instances, then there is the overhead of M times as many JVM runtimes. Moreover, if each service runs on its own VM (e.g. EC2 instance), as is the case at Netflix, the overhead is even higher.

#### Single Reponsibility (SOLID Principle)
    This means that the microservice interface should expose only access points that are relevant to the assigned function. And internally, the microservice should         have only assigned behavior.
    Providing a single responsibility means that microservices are easier to maintain and scale.
    
 #### Open Source Contribution Requirements for developers
 ##### main branch
 
 The main branch contains the code for the latest released version. We update this branch only to:
>* fix a bug present in the current version,
>* release new minor- or patch-level version.

 ##### develop branch
 
 The develop branch contains the code for the next minor version. All new features, breaking changes, and bug fixes must be merged into this branch.

 ##### To add a new feature
>* Create a new branch from the develop branch.
>* Work on the feature. 🔨
>* Create a Pull Request targeted at the develop branch following our How to submit a Pull Request guide.

##### To Fix a bug in the latest release
>* Create a new branch from the main branch.
>* Fix the bug. 🔨
>* Create a Pull Request targeted at the main branch following our How to submit a Pull Request guide.
>* If the bug is also present in the develop branch, create an additional Pull Request targeted at this branch.

##### To Fix a bug in the develop branch
>* Create a new branch from the develop branch.
>* Fix the bug. 🔨
>* Create a Pull Request targeted at the develop branch following our How to submit a Pull Request guide.

##### Submitting a pull Request
Requirements
>*  we need Yarn 1 
>* Git

To Check if you have the tools already installed or not

![middleware](https://user-images.githubusercontent.com/82566358/205516410-226976bc-bcca-44e9-9f28-972b9e288d80.png)

Steps
1.  fork our repository
2.  install all necessary dependencies/tools i.e. eslint, husky by using command yarn install
3.  Once your changes are ready, manually test them in development and production modes.
4.  If the repository contains a Vue Storefront project (often called theme), run all the build commands defined in the package.json file and start the project to test it. If everything works as expected, you can go to the next section.
5.  If there is no Vue Storefront project, create a new project using our Installation guide. Then, open its package.json file and look for the name of the package you modified in the dependencies or devDependencies. else  change the version to the link

![middleware](https://user-images.githubusercontent.com/82566358/205516617-69244759-c358-47d3-af1a-4a44f1af6146.png)

6. if it's an indirect dependency (dependency of another package) and not present in the package.json, use the Selective dependency resolutions
7. Update unit and E2E tests by openning the package.json file and see if there are one or more test commands
8. Update documentation 
9. Commit and push your changes 
10. Create Pull Request

