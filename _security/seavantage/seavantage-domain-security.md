---
api_specs:
- filename: seavantage-openapi-generated.yml
  format: yaml
  label: SeaVantage API
  slug: seavantage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/seavantage/openapi/_ae-authored/seavantage-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: seavantage.com
  spf: true
hosts:
- cert_expires: Jan 26 00:33:08 2027 GMT
  host: www.seavantage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SeaVantage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SeaVantage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SeaVantage
provider_slug: seavantage
slug: seavantage-domain-security
source_filename: seavantage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seavantage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 00:33:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: seavantage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/seavantage/security/seavantage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ocean Freight Visibility
- Cargo Tracking
- Port Congestion
- Ship AIS
- Predictive ETA
- Maritime Data
- API Integration
- Supply Chain
---
