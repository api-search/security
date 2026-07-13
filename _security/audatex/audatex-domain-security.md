---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Audatex AudaConnect API
  slug: audatex-audaconnect-api
  spec_type: OpenAPI
  url: https://audaconnect-demo.ax-aee.co.uk/AudaAPI.Bmsapi/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: audatex.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ax-aee.co.uk
  spf: false
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: www.audatex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: audaconnect-demo.ax-aee.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: api-demo.audatex.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Audatex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Audatex, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Audatex
provider_slug: audatex
slug: audatex-domain-security
source_filename: audatex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.audatex.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: audaconnect-demo.ax-aee.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: false\n- host: api-demo.audatex.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: audatex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: ax-aee.co.uk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audatex/refs/heads/main/security/audatex-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Automotive
- Claims Processing
- Insurance
- Repair Management
- Vehicle Data
---
