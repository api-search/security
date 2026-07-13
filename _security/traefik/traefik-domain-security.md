---
api_specs:
- filename: traefik-proxy-openapi.yml
  format: yaml
  label: Traefik Proxy
  slug: traefik-proxy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traefik/refs/heads/main/openapi/traefik-proxy-openapi.yml
- filename: traefik-proxy-openapi.yml
  format: yaml
  label: Traefik Proxy REST API
  slug: traefik-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traefik/refs/heads/main/openapi/traefik-proxy-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: traefik.io
  spf: true
hosts:
- cert_expires: Sep 14 04:05:11 2026 GMT
  host: traefik.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:05:11 2026 GMT
  host: doc.traefik.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:05:11 2026 GMT
  host: plugins.traefik.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Traefik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Traefik Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Traefik Labs
provider_slug: traefik
slug: traefik-domain-security
source_filename: traefik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: traefik.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:05:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: doc.traefik.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:05:11 2026 GMT\n  hsts: false\n- host: plugins.traefik.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:05:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: traefik.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traefik/refs/heads/main/security/traefik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Gateway
- API Gateway
- API Management
- Developer Portal
- GitOps
- Kubernetes
- Load Balancer
- MCP Gateway
- Open Source
- Reverse Proxy
- WAF
---
