---
api_specs:
- filename: scale3-blockchain-intelligence-openapi.yml
  format: yaml
  label: Scale3 Blockchain Intelligence API
  slug: scale3-blockchain-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale3/refs/heads/main/openapi/scale3-blockchain-intelligence-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: scale3labs.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: scale3production.com
  spf: false
hosts:
- cert_expires: Sep  6 14:13:54 2026 GMT
  host: www.scale3labs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: web-backend.scale3production.com
  https: false
kind: domain-security
layout: security
method: probed
name: Scale3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scale3, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Scale3
provider_slug: scale3
slug: scale3-domain-security
source_filename: scale3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scale3labs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 14:13:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: web-backend.scale3production.com\n  https: false\ndomains:\n- domain: scale3labs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: scale3production.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scale3/refs/heads/main/security/scale3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Web3
- Node Monitoring
- Observability
- Infrastructure
- Validators
- DevOps
- Alerting
- LLM Observability
---
