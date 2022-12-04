## Vue Store Front

### Introduction
Vue Storefront is a standalone Progressive Web Application solution for web stores that can drastically enhance the shopping experience. Moreover, thanks to the ability to connect to an array of eCommerce backend solutions like Magento, Prestashop or Shopware through their respective API, it can be used by any store.  It can also serve as a great code base for developers who build front-end for eCommerce stores. 

### Installation
 To set Up VueStoreFront on your local environment you must have to fulfill the following system requirements.
 
 #### Prerequisites
 
>* Node.js latest version This includes a version manager, package manager, and Visual Studio Code. The Node Package Manager (npm) is used to install Vue.js.
>* Vue.js framework
>* Express.js for Server API
>* Elastic Search
>* Docker

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
