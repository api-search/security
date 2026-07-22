---
api_specs:
- filename: nimbleway-openapi.json
  format: json
  label: Nimble SDK
  slug: nimble-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/openapi/nimbleway-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nimbleway.com
  spf: true
hosts:
- cert_expires: Oct 14 23:48:24 2026 GMT
  host: nimbleway.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 06:19:50 2026 GMT
  host: sdk.nimbleway.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nimbleway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nimbleway, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nimbleway
provider_slug: nimbleway
slug: nimbleway-domain-security
source_filename: nimbleway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nimbleway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:48:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sdk.nimbleway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 06:19:50 2026 GMT\n  hsts: null\ndomains:\n- domain: nimbleway.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nimbleway/refs/heads/main/security/nimbleway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Web Data
- Web Scraping
- Data Extraction
- Web Search
- Proxies
- AI Agents
- Model Context Protocol
---
