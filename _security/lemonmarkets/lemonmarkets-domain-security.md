---
api_specs:
- filename: lemonmarkets-brokerage-openapi.json
  format: json
  label: lemon.markets Brokerage API
  slug: brokerage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-brokerage-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lemon.markets
  spf: true
hosts:
- cert_expires: Sep 20 04:27:37 2026 GMT
  host: www.lemon.markets
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
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.lemon.markets
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lemonmarkets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lemon.markets, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: lemon.markets
provider_slug: lemonmarkets
slug: lemonmarkets-domain-security
source_filename: lemonmarkets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lemon.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 04:27:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.lemon.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:31:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lemon.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lemon.markets\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/security/lemonmarkets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Brokerage
- Investing
- Trading
- Embedded Finance
- Banking as a Service
- Securities
- Wealth Management
- Germany
- Europe
---
