# mac-apigateway-zuul

1. Start Eureka, `mac-service-registry` and services, `mac-user-service`. From https://github.com/MacKittipat/mac-service-discovery
2. Start zuul, `mac-apigateway-zuul`
3. Call `http://localhost:8080/user-service/users`
    * `user-service` is service name from `mac-service-registry`
    * `users` is REST uri from `mac-user-service`
4. Call `http://localhost:8080/user-api/users`
    * `user-api` is path config from `mac-apigateway-zuul/src/main/resources/application.yml`
    * `users` is REST uri from `mac-user-service`