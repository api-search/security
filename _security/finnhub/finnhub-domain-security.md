---
api_specs:
- filename: finnhub-asyncapi.yml
  format: yaml
  label: Finnhub
  slug: finnhub
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/finnhub/refs/heads/main/asyncapi/finnhub-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: finnhub.io
  spf: true
hosts:
- cert_expires: Aug 17 18:17:14 2026 GMT
  host: finnhub.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Finnhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finnhub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Finnhub
provider_slug: finnhub
slug: finnhub-domain-security
source_filename: finnhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finnhub.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 17 18:17:14 2026 GMT\n  hsts: null\ndomains:\n- domain: finnhub.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finnhub/refs/heads/main/security/finnhub-domain-security.yml
summary_line: TLSv1.2
tags:
- Financial
- Market Data
- Stocks
---
