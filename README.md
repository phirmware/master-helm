## First create a service account Tiller for Helm

RUN - `kubectl apply -f ./helm-rbac.yaml`

## Initialize Helm and Tiller

RUN - `helm init --service-account tiller`

## To view the pod in the kube-system namespace

RUN - `kubectl get pods -n kube-system`

## Give nodes the neccessary permissions to create DNS Records on Route53

RUN - `./put-node-policy.sh`

