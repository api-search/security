---
api_specs:
- filename: rentle-admin-openapi.json
  format: json
  label: Twice Admin API
  slug: twice-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/openapi/rentle-admin-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: twicecommerce.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rentle.io
  spf: true
hosts:
- cert_expires: Aug 21 14:10:42 2026 GMT
  host: www.twicecommerce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 21:10:39 2026 GMT
  host: api.rentle.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 09:55:00 2026 GMT
  host: api.twicecommerce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rentle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rentle, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rentle
provider_slug: rentle
slug: rentle-domain-security
source_filename: rentle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.twicecommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 14:10:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rentle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:10:39 2026 GMT\n  hsts: null\n- host: api.twicecommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 09:55:00 2026 GMT\n  hsts: null\ndomains:\n- domain: twicecommerce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rentle.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/security/rentle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Rental
- Commerce
- E-commerce
- Circular Economy
- Resale
- Subscriptions
- Bookings
- Webhooks
- SaaS
---
