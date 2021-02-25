.PHONY: configmap

configmap:
	-kubectl delete configmap ucsdoriginconfig -n cms-admin
	kubectl create configmap ucsdoriginconfig -n cms-admin --from-file=95-local-ucsd.cfg

secrets:
	-kubectl delete secret ucsd-origin-certs -n cms-admin
	kubectl create secret generic ucsd-origin-certs -n cms-admin --from-file=hostcert=hostcert.pem --from-file=hostkey=hostkey.pem

