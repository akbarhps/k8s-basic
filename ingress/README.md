NOTE:

For Windows:
- After apply the ingress controller, you need to run `minikube tunnel` because of this [known issue](https://minikube.sigs.k8s.io/docs/drivers/docker/#known-issues)
- After that, you have to set the host to hosts file, because:
`You need to setup your /etc/hosts, I guess the ingress controller wait for requests with an host defined to redirect them, but it's pretty strange that it didn't even respond to the http request with an error.` [source](https://stackoverflow.com/questions/70366074/ingress-not-working-from-official-kubernetes-tutorial/70382920#70382920)
- Then you can access the page via browser using the ingress host