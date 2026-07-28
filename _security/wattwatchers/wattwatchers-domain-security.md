---
api_specs:
- filename: wattwatchers-rest-api-v3-openapi.json
  format: json
  label: Wattwatchers REST API v3 (Mercury)
  slug: wattwatchers-rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wattwatchers/refs/heads/main/openapi/wattwatchers-rest-api-v3-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wattwatchers.com.au
  spf: true
hosts:
- cert_expires: Sep 12 17:16:40 2026 GMT
  host: wattwatchers.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: docs.wattwatchers.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api-v3.wattwatchers.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wattwatchers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wattwatchers, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wattwatchers
provider_slug: wattwatchers
slug: wattwatchers-domain-security
source_filename: wattwatchers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wattwatchers.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 17:16:40 2026 GMT\n  hsts: false\n- host: docs.wattwatchers.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\n- host: api-v3.wattwatchers.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wattwatchers.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wattwatchers/refs/heads/main/security/wattwatchers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Smart Metering
- Energy Data
- IoT
- Solar
- DER
- Demand Response
---
