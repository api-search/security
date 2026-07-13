---
api_specs:
- filename: enable-banking-api-openapi.yml
  format: yaml
  label: Enable Banking API
  slug: enable-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enable-banking/refs/heads/main/openapi/enable-banking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: enablebanking.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: tilisy.com
  spf: true
hosts:
- cert_expires: Oct  1 13:44:00 2026 GMT
  host: enablebanking.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 02:01:20 2026 GMT
  host: api.enablebanking.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 16:48:38 2026 GMT
  host: api.tilisy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enable Banking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enable Banking, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Enable Banking
provider_slug: enable-banking
slug: enable-banking-domain-security
source_filename: enable-banking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enablebanking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 13:44:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.enablebanking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 02:01:20 2026 GMT\n  hsts: null\n- host: api.tilisy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 16:48:38 2026 GMT\n  hsts: null\ndomains:\n- domain: enablebanking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tilisy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enable-banking/refs/heads/main/security/enable-banking-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Banking
- PSD2
- AISP
- PISP
- Banking
- Financial Services
- Account Aggregation
- Payment Initiation
- Europe
- Nordic
- Finland
- Compliance
- eIDAS
- SCA
- DORA
- GDPR
---
