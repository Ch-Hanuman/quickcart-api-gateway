# api-gateway
Spring Cloud Gateway, port **8080**. Routes `/api/products/**` → inventory-service and `/api/orders/**` → order-service
via Eureka (`lb://`). Internal `/api/inventory/**` is deliberately not exposed.
Build: `docker build -t quickcart/api-gateway:1.0.0 .` · Deploy: `kubectl apply -f k8s/` (NodePort 30080)
