# istio-restricted
istio installation for restricted kubernetes clusters

Components:
|istio-injector | :white_check_mark:|
|istio-cni|:white_check_mark:|
|istio-citadel|:white_check_mark:|
|istio-pilot|:white_check_mark:|
|istio-ingressgateway|:white_check_mark:|
|istio-policy|:black_square_button:|
|istio-telemetry|:black_square_button:|
|zipkin/jaeger|:black_square_button:|
|istio-galley|:black_square_button:|
|istio-nodeagent|:skull:|
|kiali|:black_square_button:|



cluster-admin role:
kubectl apply -f system

namespace admin role:
kubectl --nammespace=myns apply -f userns

Examples:
kubectl --namespace=myns apply -f https://raw.githubusercontent.com/istio/istio/release-1.4/samples/bookinfo/platform/kube/bookinfo.yaml
kubectl --namespace=myns apply -f examples

