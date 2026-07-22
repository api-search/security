---
api_specs:
- filename: slope-software-openapi-original.json
  format: json
  label: Slope API
  slug: slope-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slope-software/refs/heads/main/openapi/slope-software-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: slopesoftware.com
  spf: true
hosts:
- cert_expires: Sep 28 06:28:33 2026 GMT
  host: slopesoftware.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: api.slopesoftware.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slope Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slope Software, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Slope Software
provider_slug: slope-software
slug: slope-software-domain-security
source_filename: slope-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: slopesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 06:28:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.slopesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: slopesoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slope-software/refs/heads/main/security/slope-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Actuarial
- Insurance
- Actuarial Modeling
- Valuation
- Financial Services
- Life Insurance
- Annuities
- Pension
- Risk Management
- Cloud
- Reporting
---
