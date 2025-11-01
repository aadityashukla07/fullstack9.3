Application Load Balancer (ALB) Setup Create an ALB in the EC2 Console:

Scheme: internet-facing Listeners: HTTP (80) and optionally HTTPS (443) Availability Zones: Select multiple AZs Create a Target Group:

Target type: instance Protocol: HTTP Port: 5000 Health check path: /health Healthy threshold: 2, Unhealthy threshold: 3, Timeout: 5s, Interval: 30s Register backend EC2 instances with the Target Group.

Add listener rule to forward incoming traffic to the Target Group.

(Optional) Configure HTTPS using ACM certificate and add 443 listener.
