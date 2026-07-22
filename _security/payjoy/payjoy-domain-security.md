---
api_specs:
- filename: payjoy-partner-api-openapi.yml
  format: yaml
  label: PayJoy Partner API V2 (Sales Integration)
  slug: payjoy-partner-api-v2-sales-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjoy/refs/heads/main/openapi/payjoy-partner-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: payjoy.com
  spf: true
hosts:
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: www.payjoy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 01:58:03 2026 GMT
  host: developers.payjoy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: partner-integration.sandbox.payjoy.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Payjoy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayJoy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PayJoy
provider_slug: payjoy
slug: payjoy-domain-security
source_filename: payjoy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.payjoy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: false\n- host: developers.payjoy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 01:58:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner-integration.sandbox.payjoy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: payjoy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payjoy/refs/heads/main/security/payjoy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Lending
- Buy Now Pay Later
- Point of Sale
- Emerging Markets
- Financial Inclusion
- Partner API
---
