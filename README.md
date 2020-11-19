# CPAT IBM guardian operator

<b>This operator allows you to track configmap creation, updates from a remote git repository.</b>

To quickly test this operator you can add the custom catalog source from this repository:

<b>oc create -f catalog_source.yaml -n openshift-marketplace</b>

Then the operator will appear in Operatorhub catalog..

You will need to also apply the 2 CRDs in this repository(@TODO find a way to package it with the operator)
The CRDs can be found here: (https://github.com/gregmeszaros/cpat-ibm-guardian-operator/tree/master/deploy/crds)
