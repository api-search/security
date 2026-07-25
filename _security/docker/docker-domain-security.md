---
api_specs:
- filename: docker-config-api-openapi.yml
  format: yaml
  label: Docker Config API
  slug: docker-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-config-api-openapi.yml
- filename: docker-container-api-openapi.yml
  format: yaml
  label: Docker Container API
  slug: docker-container-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-container-api-openapi.yml
- filename: docker-distribution-api-openapi.yml
  format: yaml
  label: Docker Distribution API
  slug: docker-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-distribution-api-openapi.yml
- filename: docker-exec-api-openapi.yml
  format: yaml
  label: Docker Exec API
  slug: docker-exec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-exec-api-openapi.yml
- filename: docker-image-api-openapi.yml
  format: yaml
  label: Docker Image API
  slug: docker-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-image-api-openapi.yml
- filename: docker-network-api-openapi.yml
  format: yaml
  label: Docker Network API
  slug: docker-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-network-api-openapi.yml
- filename: docker-node-api-openapi.yml
  format: yaml
  label: Docker Node API
  slug: docker-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-node-api-openapi.yml
- filename: docker-plugin-api-openapi.yml
  format: yaml
  label: Docker Plugin API
  slug: docker-plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-plugin-api-openapi.yml
- filename: docker-secret-api-openapi.yml
  format: yaml
  label: Docker Secret API
  slug: docker-secret-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-secret-api-openapi.yml
- filename: docker-service-api-openapi.yml
  format: yaml
  label: Docker Service API
  slug: docker-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-service-api-openapi.yml
- filename: docker-session-api-openapi.yml
  format: yaml
  label: Docker Session API
  slug: docker-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-session-api-openapi.yml
- filename: docker-swarm-api-openapi.yml
  format: yaml
  label: Docker Swarm API
  slug: docker-swarm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-swarm-api-openapi.yml
- filename: docker-system-api-openapi.yml
  format: yaml
  label: Docker System API
  slug: docker-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-system-api-openapi.yml
- filename: docker-task-api-openapi.yml
  format: yaml
  label: Docker Task API
  slug: docker-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-task-api-openapi.yml
- filename: docker-volume-api-openapi.yml
  format: yaml
  label: Docker Volume API
  slug: docker-volume-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-volume-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:infra+caa-iodef@docker.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: docker.com
  spf: true
hosts:
- cert_expires: Aug 29 10:28:18 2026 GMT
  host: www.docker.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Docker
provider_slug: docker
slug: docker-domain-security
source_filename: docker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.docker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 10:28:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: docker.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:infra+caa-iodef@docker.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/security/docker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Containers
- DevOps
- Infrastructure
- Microservices
---
