# docker_jupyter_r-notebook_rstan
RStan in Docker jupyter/r-notebook

See the log of the unsuccessful install at http://htmlpreview.github.io/?https://github.com/gaborgulya/docker_jupyter_r-notebook_rstan/blob/master/Install%20and%20test%20RStan%20-%20failed.html . Ben Goodrich has kindly helped: http://discourse.mc-stan.org/t/unsuccessful-install-of-rstan-in-docker-jupyter-r-notebook/2588/2 .

What I had to do was both give sufficient RAM to docker (2GB was not enough, 6Gb was), and also compile Rcpp: http://htmlpreview.github.io/?https://github.com/gaborgulya/docker_jupyter_r-notebook_rstan/blob/master/Install%20and%20test%20RStan%20-%20succeeded.html

Planned steps:
 * Automate the install of Rcpp and RStan in a Dockerfile extending jupyter/r-notebook
 * Share the Dockerfile at docker.com
