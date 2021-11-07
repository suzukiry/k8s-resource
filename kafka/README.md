
oc logs $(oc get pod -l name=kafka-producer -o=jsonpath='{.items[0].metadata.name}') -f

oc logs $(oc get pod -l name=kafka-consumer -o=jsonpath='{.items[0].metadata.name}') -f

