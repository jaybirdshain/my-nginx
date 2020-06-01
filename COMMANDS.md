helm list
helm get all my-nginx
helm upgrade my-nginx . --set service.type=NodePort
helm upgrade my-nginx . --set service.type=LoadBalancer #overrides the service type
helm upgrade my-nginx . #same as above
helm rollback 2 #rolls back to this version
helm delete --purge my-nginx #sometimes --purge is not an option?


