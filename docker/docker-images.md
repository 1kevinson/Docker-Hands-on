<!-- @format -->

## Docker ps commands

---

**GOOD TO KNOW** : we cannot remove a image which have a container dependency (_remove the container first_)

see the image I currrently have

> docker images

remove image by name or id

> docker rmi `name`

> docker rmi `id`


to build a image (refer to the dockerfile in the same folder)
> docker build .

set image tag ( Repostiry name in `docker images`)
> docker build . -t my-custom-webapp