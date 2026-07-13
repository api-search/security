---
api_specs:
- filename: chickfila-bovine.yml
  format: yaml
  label: Chick-fil-A BOVINE
  slug: chick-fil-a-bovine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chickfila/refs/heads/main/openapi/chickfila-bovine.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chick-fil-a.com
  spf: true
hosts:
- cert_expires: Aug 28 10:56:40 2026 GMT
  host: www.chick-fil-a.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 21:58:46 2026 GMT
  host: order.chick-fil-a.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chickfila Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chick-fil-A, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chick-fil-A
provider_slug: chickfila
slug: chickfila-domain-security
source_filename: chickfila-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chick-fil-a.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 10:56:40 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: order.chick-fil-a.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:58:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chick-fil-a.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chickfila/refs/heads/main/security/chickfila-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fast Food
- Restaurants
- Food & Beverage
- Loyalty
- Mobile Ordering
- Catering
---
