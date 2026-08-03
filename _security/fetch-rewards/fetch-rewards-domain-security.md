---
api_specs:
- filename: fetch-rewards-receipt-processor-openapi.yml
  format: yaml
  label: Fetch Receipt Processor (Reference Specification)
  slug: receipt-processor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fetch-rewards/refs/heads/main/openapi/fetch-rewards-receipt-processor-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fetch.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: fetch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fetch Rewards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fetch Rewards, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fetch Rewards
provider_slug: fetch-rewards
slug: fetch-rewards-domain-security
source_filename: fetch-rewards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fetch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: fetch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fetch-rewards/refs/heads/main/security/fetch-rewards-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Rewards
- Loyalty
- Consumer
- Retail
- Advertising
- Receipts
- Consumer Packaged Goods
- Mobile
- Marketing
---
