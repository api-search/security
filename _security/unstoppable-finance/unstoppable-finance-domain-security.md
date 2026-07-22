---
api_specs:
- filename: unstoppable-finance-iron-openapi-original.yml
  format: yaml
  label: Iron API
  slug: iron-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-finance/refs/heads/main/openapi/unstoppable-finance-iron-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iron.xyz
  spf: true
hosts:
- cert_expires: Sep 15 06:49:32 2026 GMT
  host: iron.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 12:16:58 2026 GMT
  host: docs.iron.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 18:44:24 2026 GMT
  host: api.iron.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unstoppable Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unstoppable Finance (Iron), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unstoppable Finance (Iron)
provider_slug: unstoppable-finance
slug: unstoppable-finance-domain-security
source_filename: unstoppable-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iron.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:49:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.iron.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:16:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.iron.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 18:44:24 2026 GMT\n  hsts: false\ndomains:\n- domain: iron.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unstoppable-finance/refs/heads/main/security/unstoppable-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Stablecoins
- Payments
- Onramp
- Offramp
- Cryptocurrency
- Banking
- Fintech
- Compliance
---
