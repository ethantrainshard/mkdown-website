---
tags:
    - Docker
    - CloudFlare
    - Step-By-Step
---

# CloudFlare Tunnel

## Description
A Cloudflare Tunnel allows developers to securely expose any internal service or application behind their firewall to the public internet without having to make significant changes to their infrastructure. This is achieved through Cloudflare's edge network, which acts as a secure tunnel between the user's browser and your internal service. It helps you achieve a better balance between security, performance, and simplicity while exposing your internal resources to the public internet.

## Key Features

- Zero-Trust Access: Only allow access to specific resources on your internal network.
- Security: Leverage Cloudflare's global security infrastructure (firewalls, SSL/TLS encryption, etc.) for enhanced protection.
- Performance: Enjoy improved performance and lower latency by serving content directly from the edge.

## Uses

- Exposing Internal Services to the Public Internet: Connect your internal services to the public internet securely.
- Webhook Endpoints: Protect webhook endpoints and API calls with Cloudflare's edge security capabilities.
- Reverse Proxies: Set up reverse proxies for custom domains, subdomains, or paths.

## Benefits

1. **Simplified Security Configuration**: Focus on your application's core logic without worrying about network-level security complexities.
2. **Improved Performance**: Get the fastest possible access to your internal services with the edge network serving content directly from Cloudflare's global locations.
3. **Reduced Infrastructure Overhead**: Avoid managing additional infrastructure or software for secure exposure.

## Network Diagram

## Installation

### Linux / Macos

### Docker

```bash title="Setting Environment Variable"
export TUNNEL_TOKEN={TUNNEL_TOKEN}
```

```bash
docker-compose up -d
```