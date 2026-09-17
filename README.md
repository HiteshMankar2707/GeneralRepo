## Technical term — short
port → Service port — the port on which the Kubernetes Service accepts traffic.
targetPort → Backend/Pod port — the port on which the application inside the Pod receives traffic.

## Example:
port: 80
targetPort: 8080
Client → Service:80 → Pod:8080 → Application

## If NLB supports TCP/UDP, why can't standard Ingress handle TCP/UDP?"
"NLB is a Layer-4 load balancer and can handle TCP and UDP. Kubernetes Ingress, however, is a Layer-7 API designed primarily for HTTP/HTTPS routing. When NLB is used with an NGINX Ingress Controller, NLB provides the external Layer-4 entry point, while NGINX handles HTTP/HTTPS Ingress rules. NGINX can also expose TCP/UDP through controller-specific configuration, but those TCP/UDP routes are not defined by the standard Ingress resource."

## Binlog 
Binlog is a MySQL binary log that records database changes such as INSERT, UPDATE, and DELETE. It is commonly used for replication, point-in-time recovery, and change data capture."

## MYSQL Login 
mysql -u admin -h <EndPoint> -P 3306 -p      ->>> -p (Small p is password & P capital P is port)
