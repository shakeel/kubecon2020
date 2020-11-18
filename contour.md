# Contour, A High Performance Multitenant Ingress Controller for Kubernetes

Contour, a CNCF incubating project, is a high performance ingress and load balancer solution for Kubernetes. 

Contour offers a richer feature set than some common alternatives while maintaining a lightweight profile. 

At its core, Contour is providing a control plane for the Envoy edge and service proxy. 

This session will show you how to leverage Contour and Envoy for Kubernetes workloads in a multi-tenant environment, demonstrate recent Contour features like authentication and preview our near term roadmap.

## Links

* https://projectcontour.io/
* https://projectcontour.io/docs/v1.10.0/config/client-authorization/
* https://github.com/projectcontour/contour
* https://github.com/bitnami/charts/tree/master/bitnami/contour
* https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/1.2/vmware-tanzu-kubernetes-grid-12/GUID-extensions-ingress-contour.html?hWord=N4IghgNiBcIJYDsDmAnApgZwyAvkA

## Demo of Auth service in the Ingress controller

```
kubectl get proxy -A

```

* Cluster running with Contour deployed to it.
* Deploy a namespace
* In the namespace create secrets
* Create a basic password auth service
* Create a cluster issuer for the auth service
* Deploy the auth service which is htpasswd and the authserver docker image from the Contour project.
* Deploy auth service and certificates to the cluster.
* For the secrets we need some database with user passwords.
* Deploy extension service which uses the auth service.
* Now inform the http proxy to use the auth service via the extension service.
* Envoy will then authenticate all requests to the services in our cluster.
* And then when you do a curl request, you will get a 401 redirect without a password.
* In your application routes you can apply auth policy to secure some parts of your app.

## Rate Limiting

Rate limit particular routes or services.

## Deployment Support

Helm chart and Operator

## Roadmap

https://github.com/projectcontour/community/blob/main/ROADMAP.md


