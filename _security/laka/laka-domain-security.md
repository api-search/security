---
api_specs:
- filename: laka-platform-openapi.json
  format: json
  label: Laka Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laka/refs/heads/main/openapi/laka-platform-openapi.json
- filename: laka-quote-openapi.json
  format: json
  label: Laka Quote API
  slug: quote
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laka/refs/heads/main/openapi/laka-quote-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: laka.co
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: laka.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 11:11:46 2026 GMT
  host: docs.laka.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: api-gb.app.laka.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Laka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laka, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Laka
provider_slug: laka
slug: laka-domain-security
source_filename: laka-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laka.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.laka.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 11:11:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-gb.app.laka.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: laka.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laka/refs/heads/main/security/laka-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- InsurTech
- Cycling
- Micro Mobility
- Bicycle Insurance
- Claims
- Policies
- Quotes
- Embedded Insurance
- Europe
---
