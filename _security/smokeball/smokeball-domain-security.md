---
api_specs:
- filename: openapi.json
  format: json
  label: Smokeball API
  slug: smokeball-api
  spec_type: OpenAPI
  url: https://docs.smokeball.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smokeball.com
  spf: true
hosts:
- cert_expires: Aug 17 10:54:15 2026 GMT
  host: www.smokeball.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:16 2026 GMT
  host: docs.smokeball.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.smokeball.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smokeball Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smokeball, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Smokeball
provider_slug: smokeball
slug: smokeball-domain-security
source_filename: smokeball-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smokeball.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 10:54:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.smokeball.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.smokeball.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: smokeball.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smokeball/refs/heads/main/security/smokeball-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- Law Firm
- Practice Management
- Matters
- Contacts
- Documents
- Billing
- Trust Accounting
- Time Tracking
---
