---
api_specs:
- filename: forex-openapi.yml
  format: yaml
  label: Open Exchange Rates API
  slug: open-exchange-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forex/refs/heads/main/openapi/forex-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openexchangerates.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fixer.io
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: openexchangerates.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  4 02:46:34 2026 GMT
  host: fixer.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 02:46:34 2026 GMT
  host: api.fixer.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forex, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Forex
provider_slug: forex
slug: forex-domain-security
source_filename: forex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openexchangerates.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: fixer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:46:34 2026 GMT\n  hsts: false\n- host: api.fixer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:46:34 2026 GMT\n  hsts: false\ndomains:\n- domain: openexchangerates.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: fixer.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forex/refs/heads/main/security/forex-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Currency
- Exchange Rates
- Financial Data
- Forex
- Trading
---
