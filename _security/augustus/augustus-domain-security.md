---
api_specs:
- filename: augustus-openapi-original.yml
  format: yaml
  label: Augustus Banking API
  slug: augustus-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: augustus.com
  spf: true
hosts:
- cert_expires: Oct  8 17:43:06 2026 GMT
  host: augustus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 09:25:51 2026 GMT
  host: docs.augustus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: api.augustus.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Augustus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Augustus, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Augustus
provider_slug: augustus
slug: augustus-domain-security
source_filename: augustus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: augustus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 17:43:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.augustus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:25:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.augustus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: augustus.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/security/augustus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Payments
- Banking
- Open Banking
- Stablecoin
- Payouts
- Foreign Exchange
- Webhooks
---
