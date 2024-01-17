# poc-ksops
Playing with ksops
age-keygen -o age.agekey
cat age.agekey | oc create secret generic sops-age --namespace=openshift-gitops --from-file=key.txt=/dev/stdin
