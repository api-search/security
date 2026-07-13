---
api_specs:
- filename: docker-openapi.yml
  format: yaml
  label: Docker
  slug: docker
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker/refs/heads/main/openapi/docker-openapi.yml
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
