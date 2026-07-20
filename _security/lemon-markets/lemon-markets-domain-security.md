---
api_specs:
- filename: lemon-markets-brokerage-openapi.json
  format: json
  label: lemon.markets Brokerage API
  slug: brokerage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemon-markets/refs/heads/main/openapi/lemon-markets-brokerage-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lemon.markets
  spf: true
hosts:
- cert_expires: Sep 15 04:32:35 2026 GMT
  host: lemon.markets
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 07:31:01 2026 GMT
  host: developer.lemon.markets
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: sandbox.api.lemon.markets
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lemon Markets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lemon Markets, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lemon Markets
provider_slug: lemon-markets
slug: lemon-markets-domain-security
source_filename: lemon-markets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lemon.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:32:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.lemon.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:31:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.api.lemon.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lemon.markets\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemon-markets/refs/heads/main/security/lemon-markets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Brokerage
- Trading
- Investing
- Securities
- Financial Services
- Banking as a Service
- Fintech
- Wealth Management
- Embedded Finance
- Germany
---
