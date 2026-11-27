---
api_specs:
- filename: marketheist-io-api-openapi.json
  format: json
  label: MarketHeist Backtest API API
  slug: marketheist-backtest-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/marketheist-io/openapi/_original/marketheist-io-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: marketheist.io
  spf: true
hosts:
- cert_expires: Jan 17 18:05:51 2027 GMT
  host: marketheist.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MarketHeist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarketHeist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MarketHeist
provider_slug: marketheist-io
slug: marketheist-io-domain-security
source_filename: marketheist-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marketheist.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 18:05:51 2027 GMT\n  hsts: false\ndomains:\n- domain: marketheist.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/marketheist-io/security/marketheist-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Finance
- Investment
- Portfolio
- Backtesting
---
