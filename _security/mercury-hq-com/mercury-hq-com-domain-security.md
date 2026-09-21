---
api_specs:
- filename: mercury-hq-com-x402-storefront-openapi.yml
  format: yaml
  label: MERCURY x402 Storefront API
  slug: mercury-x402-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercury-hq-com/refs/heads/main/openapi/mercury-hq-com-x402-storefront-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mercury-hq.com
  spf: false
hosts:
- cert_expires: Nov  5 11:40:30 2026 GMT
  host: mercury-hq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 11:41:42 2026 GMT
  host: network.mercury-hq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Mercury Hq Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MERCURY, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MERCURY
provider_slug: mercury-hq-com
slug: mercury-hq-com-domain-security
source_filename: mercury-hq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mercury-hq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 11:40:30 2026 GMT\n  hsts: false\n- host: network.mercury-hq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 11:41:42 2026 GMT\n  hsts: false\ndomains:\n- domain: mercury-hq.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercury-hq-com/refs/heads/main/security/mercury-hq-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Agents
- A2A
- MCP
- x402
- HTTP 402
- Machine Payments
- Web Data
- Web Scraping
- Data Extraction
- Provenance
- Stablecoins
- Artificial Intelligence
---
