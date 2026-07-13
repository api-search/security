---
api_specs:
- filename: readme-openapi.yml
  format: yaml
  label: ReadMe API
  slug: readme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-openapi.yml
- filename: readme-developer-metrics-openapi.yml
  format: yaml
  label: ReadMe Developer Metrics API
  slug: developer-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-developer-metrics-openapi.yml
- filename: readme-personalized-docs-webhook-asyncapi.yml
  format: yaml
  label: ReadMe Personalized Docs Webhook
  slug: personalized-docs-webhook
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/asyncapi/readme-personalized-docs-webhook-asyncapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.com
  spf: true
hosts:
- cert_expires: Oct  6 16:29:30 2026 GMT
  host: readme.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 07:54:10 2026 GMT
  host: docs.readme.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 22:42:46 2026 GMT
  host: api.readme.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Readme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReadMe, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ReadMe
provider_slug: readme
slug: readme-domain-security
source_filename: readme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: readme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:29:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.readme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 07:54:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.readme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 22:42:46 2026 GMT\n  hsts: null\ndomains:\n- domain: readme.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/security/readme-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Documentation
- Developer Hub
- API Reference
- Portals
- Analytics
- AI
- MCP
- Bi-Directional Sync
---
