---
api_specs:
- filename: seel-openapi.yml
  format: yaml
  label: Seel Commerce Protection API
  slug: seel-commerce-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seel/refs/heads/main/openapi/seel-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: seel.com
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: seel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api-test.seel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Seel
provider_slug: seel
slug: seel-domain-security
source_filename: seel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-test.seel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: seel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seel/refs/heads/main/security/seel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-commerce
- Insurance
- Post-Purchase
- Returns
- Extended Warranty
- Fraud
- Payments
---
