---
api_specs:
- filename: stoplight-versions-api-openapi.yml
  format: yaml
  label: Stoplight Versions API
  slug: stoplight-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stoplight/refs/heads/main/openapi/stoplight-versions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "cloudflare.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stoplight.io
  spf: true
hosts:
- cert_expires: Dec 10 04:58:48 2026 GMT
  host: stoplight.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 04:58:48 2026 GMT
  host: docs.stoplight.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 04:58:48 2026 GMT
  host: api.stoplight.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Stoplight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stoplight, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stoplight
provider_slug: stoplight
slug: stoplight-domain-security
source_filename: stoplight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 04:58:48 2026 GMT\n  hsts: false\n- host: docs.stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 04:58:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 04:58:48 2026 GMT\n  hsts: null\ndomains:\n- domain: stoplight.io\n  dnssec: false\n  caa:\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stoplight/refs/heads/main/security/stoplight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Design
- API Documentation
- API Governance
- AsyncAPI
- Design-First
- Developer Tools
- Linting
- Mock Servers
- OpenAPI
- SmartBear API Hub
- Style Guides
---
