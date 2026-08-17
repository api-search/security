---
api_specs:
- filename: broadlume-bms-openapi.yml
  format: yaml
  label: Broadlume BMS API
  slug: bms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadlume/refs/heads/main/openapi/broadlume-bms-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: broadlume.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rmaster.com
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: broadlume.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 12:14:46 2026 GMT
  host: developer.broadlume.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.rmaster.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Broadlume Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Broadlume, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Broadlume
provider_slug: broadlume
slug: broadlume-domain-security
source_filename: broadlume-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: broadlume.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.broadlume.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 12:14:46 2026 GMT\n  hsts: null\n- host: api.rmaster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: broadlume.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rmaster.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/broadlume/refs/heads/main/security/broadlume-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Flooring
- Retail
- Marketing
- Websites
- Business Software
- Home Improvement
- ERP
- Inventory
- Point of Sale
- Accounting
- Order Management
---
