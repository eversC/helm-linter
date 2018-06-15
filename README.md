# helm-linter
It:
 
* is a little Helm linter in docker.
* is based on Alpine
* just has Helm installed; any `helm lint` will need to be done by opening a shell, and running `lint` on a mounted helm dir

you can find the docker image [here](https://hub.docker.com/r/eversc/helm-linter/)

version numbers contain the Helm version followed by the base Alpine version

of course, feel free to run anything else `helm` based, though if you want to run anything that involves connecting to a kubernetes cluster / tiller (e.g. `helm init`), you may want to use a different image, e.g. [gcloud-k8s-helm](https://hub.docker.com/r/eversc/gcloud-k8s-helm/) 