# kubernetes-kafka-rest-proxy

Forking and upgraded from https://gitlab.com/atkozhuharov/kafka-rest-proxy-kubernetes

# Usage
1. Setup you Kafka cluster with server endpoint (Username, Password, SASL method if any)
2. Fill the detail in `kafka-rest-config.properties` and create secret via `kubectl create secret generic kafka-rest-config --from-file kafka-rest-config.properties`
3. Deploy Kafka Rest Proxy `kubectl apply -f https://github.com/halfjuice/kubernetes-kafka-rest-proxy/blob/main/kafka-rest-proxy-deployment.yaml`
