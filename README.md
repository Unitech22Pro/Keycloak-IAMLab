## 🛡️ Identity and Access Management Lab (Keycloak) 
⬇️See Screenshots for Steps🤓)

[View Steps & Screenshots](https://github.com/Unitech22Pro/Keycloak-IAMLab/tree/main/screenshots)

This lab simulates an IAM solution using [Keycloak](https://www.keycloak.org/) deployed locally via Docker.

### 🔧 Features
- Keycloak deployed in Docker container
- Realm and client configuration
- User creation with role-based access
- Simulated login request using `curl`
- Access token retrieved via OpenID Connect flow

### 📸 Token Retrieval Example

```bash
curl -X POST "http://localhost:8080/realms/IAM-Lab/protocol/openid-connect/token" \
  -H "Content-Type: application/x-www-form-urlencoded" \
  -d "client_id=demo-app" \
  -d "grant_type=password" \
  -d "username=YOUR_USERNAME" \
  -d "password=YOUR_PASSWORD"
