# vector 

- Replace the namespace configured across yaml files prior to executing them.

- Create the resources in the following order:

oc apply -f namespace.yaml
oc apply -f serviceaccount.yaml
oc apply -f clusterrole.yaml
oc apply -f clusterrolebinding.yaml
oc apply -f scc.yaml
oc apply -f vector-aggregator-conf.yaml
oc apply -f vector-agent-conf.yaml
oc apply -f deployment.yaml
oc apply -f service.yaml
oc apply -f daemonset.yaml

