#Repotest

This page explain the procedure how to build rshiny apps to build on a single container and connect the traffic to master container. 

Nginx is used for the reverse proxy connection as well as the landing page. 

Currently the child containers will expose port starts from 3001, 3002, 3003 and so on, this is only needed for debugging purpose. 

Once it move to production, change the port for child containers internally. Because internal port communications is sufficient. 

```
expose 
  3232
```

We will build the actual Nasqar from the same setup and this avoid more complexity in making every package in a single container. 

Next :- We will see how the multi thread will working in docker to save time in docker build process
     :- Then try to lightweight/reduce the package list to minimal to save build time.


