---
api_specs:
- filename: natural-ai-openapi-original.json
  format: json
  label: Natural API
  slug: natural-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: natural.com
  spf: true
hosts:
- cert_expires: Oct  5 21:02:56 2026 GMT
  host: www.natural.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 01:47:39 2026 GMT
  host: docs.natural.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: api.natural.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Natural Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Natural AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Natural AI
provider_slug: natural-ai
slug: natural-ai-domain-security
source_filename: natural-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.natural.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:02:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.natural.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:47:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.natural.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: natural.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/security/natural-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Payments
- Agents
- Fintech
- Money Movement
- Wallets
- Agentic Payments
- MCP
---
