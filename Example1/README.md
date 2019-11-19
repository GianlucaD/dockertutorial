** Help for Deployment**

** build the image **

`docker build -t example1 .`
example1 is the name of the image...

Image is build.

`docker images`

you should see 2 images:

``` 
example1            latest              a04200e0b8cb        7 seconds ago       165MB
httpd               2.4                 d3017f59d5e2        2 weeks ago         165MB
```
if you run docker images again you should see 4 images...

```
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
example1            latest              ebc3d60ad874        7 seconds ago       129MB
<none>              <none>              a04200e0b8cb        7 minutes ago       165MB
httpd               2.4                 d3017f59d5e2        2 weeks ago         165MB
httpd               2.4-alpine          4f3b76b9d469        3 weeks ago         129MB
```

then change Dockerfile. Replace ** httpd:2.4 ** to ** httpd:2.4-alpine **
build the image again.
``