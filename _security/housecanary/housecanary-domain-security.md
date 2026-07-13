---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: HouseCanary Analytics API
  slug: housecanary-analytics-api
  spec_type: OpenAPI
  url: https://api-docs-legacy.housecanary.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: housecanary.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.housecanary.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: api.housecanary.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: order-manager-api.housecanary.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Housecanary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HouseCanary, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HouseCanary
provider_slug: housecanary
slug: housecanary-domain-security
source_filename: housecanary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.housecanary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.housecanary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: order-manager-api.housecanary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: housecanary.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/housecanary/refs/heads/main/security/housecanary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Property Analytics
- AVM
- Valuation
- Rental Estimates
- Market Forecasts
- Mortgage
- Property Data
---
