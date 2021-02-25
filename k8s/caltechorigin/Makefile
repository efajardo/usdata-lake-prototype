.PHONY: configmap

secrets:
	-kubectl delete secret caltech-origin-certs -n cms-admin
	kubectl create secret generic caltech-origin-certs -n cms-admin --from-file=hostcert=hostcert.pem --from-file=hostkey=hostkey.pem

