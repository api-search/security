---
api_specs:
- filename: involve-asia-publisher-openapi.yml
  format: yaml
  label: Involve Asia Publisher API
  slug: involve-asia-publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/involve-asia/refs/heads/main/openapi/involve-asia-publisher-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: involve.asia
  spf: true
hosts:
- cert_expires: Sep 23 15:48:15 2026 GMT
  host: involve.asia
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 15:48:15 2026 GMT
  host: api.involve.asia
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Involve Asia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Involve Asia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Involve Asia
provider_slug: involve-asia
slug: involve-asia-domain-security
source_filename: involve-asia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: involve.asia\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:48:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.involve.asia\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:48:15 2026 GMT\n  hsts: false\ndomains:\n- domain: involve.asia\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/involve-asia/refs/heads/main/security/involve-asia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Affiliate Marketing
- Performance Marketing
- Partnership Marketing
- Publishers
- Creators
- Conversions
- Deeplinks
- Commissions
- Ecommerce
- Southeast Asia
- Shopee
- Company
---
