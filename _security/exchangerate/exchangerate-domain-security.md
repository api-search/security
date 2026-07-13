---
api_specs:
- filename: exchangerate-openapi.yml
  format: yaml
  label: ExchangeRate-API
  slug: exchangerate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate/refs/heads/main/openapi/exchangerate-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: exchangerate-api.com
  spf: true
hosts:
- cert_expires: Sep 14 15:00:24 2026 GMT
  host: www.exchangerate-api.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 15:00:24 2026 GMT
  host: v6.exchangerate-api.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exchangerate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ExchangeRate-API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ExchangeRate-API
provider_slug: exchangerate
slug: exchangerate-domain-security
source_filename: exchangerate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.exchangerate-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:00:24 2026 GMT\n  hsts: false\n- host: v6.exchangerate-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:00:24 2026 GMT\n  hsts: false\ndomains:\n- domain: exchangerate-api.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exchangerate/refs/heads/main/security/exchangerate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Currency
- Exchange Rates
- Finance
- Forex
- Financial Data
- Currency Conversion
---
