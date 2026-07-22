---
api_specs:
- filename: wealth-x-connect-openapi.yml
  format: yaml
  label: Wealth-X Connect API
  slug: wealth-x-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/openapi/wealth-x-connect-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wealthx.com
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: connect.wealthx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wealth X Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wealth-X, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wealth-X
provider_slug: wealth-x
slug: wealth-x-domain-security
source_filename: wealth-x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connect.wealthx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wealthx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/security/wealth-x-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Wealth Intelligence
- Data
- UHNW
- Prospecting
- Financial Services
- CRM
- People Data
---
