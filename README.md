# portainer-installation
```
helm upgrade --install --create-namespace -n portainer portainer portainer/portainer --set service.type=ClusterIP --set tls.force=true --set ingress.enabled=true  --set ingress.ingressClassName=nginx  --set ingress.annotations."nginx\.ingress\.kubernetes\.io/backend-protocol"=HTTPS --set ingress.hosts[0].host=portainer.anaeleboo.com --set ingress.hosts[0].paths[0].path="/"
```
