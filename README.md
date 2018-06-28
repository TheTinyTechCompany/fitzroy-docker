# fitzroy-docker

A Docker image for [Fitzroy](https://github.com/jimmyday12/fitzRoy).  Get your AFL stats in a container.

#### Usage
 
Once you have the images, (e.g. `docker pull thetinytechco/fitzroy:rstudio`)

* `docker run -it thetinytechco/fitzroy:rstudio R` to start with an R terminal prompt.
* `docker run -d -p 8787:8787 --name fitzroy thetinytechco/fitzroy:rstudio` and open http://localhost:8787 for [RStudio](https://www.rstudio.com/) with Fitzroy ready to use. Username: `rstudio`, Password: `rstudio`

#### Building the image

From the root of the repo...

* Build the image
    * `docker build -t thetinytechco/fitzroy:rstudio -f rstudio/Dockerfile .`
