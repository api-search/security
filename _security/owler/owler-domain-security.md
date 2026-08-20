---
api_specs:
- filename: owler-enterprise-api-openapi.yml
  format: yaml
  label: Owler Enterprise API
  slug: owler-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/owler/refs/heads/main/openapi/owler-enterprise-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: owler.com
  spf: true
hosts:
- cert_expires: Oct 15 05:27:50 2026 GMT
  host: corp.owler.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: developers.owler.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: apiv2.owler.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Owler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Owler, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Owler
provider_slug: owler
slug: owler-domain-security
source_filename: owler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corp.owler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 05:27:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.owler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\n- host: apiv2.owler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: owler.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/owler/refs/heads/main/security/owler-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Company Intelligence
- Sales Intelligence
- Competitive Intelligence
- Business Data
- Data Licensing
- News Monitoring
- Market Research
- Firmographics
- Company Search
- funding-data
---
