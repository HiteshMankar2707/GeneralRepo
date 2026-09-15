## Technical term — short
port → Service port — the port on which the Kubernetes Service accepts traffic.
targetPort → Backend/Pod port — the port on which the application inside the Pod receives traffic.

## Example:
port: 80
targetPort: 8080
Client → Service:80 → Pod:8080 → Application
