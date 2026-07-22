---
api_specs:
- filename: powernaut-partner-api-openapi-original.yml
  format: yaml
  label: Powernaut Partner API
  slug: powernaut-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-partner-api-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: powernaut.io
  spf: true
hosts:
- cert_expires: Aug 29 16:11:24 2026 GMT
  host: powernaut.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Powernaut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Powernaut, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Powernaut
provider_slug: powernaut
slug: powernaut-domain-security
source_filename: powernaut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: powernaut.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 16:11:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: powernaut.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/security/powernaut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Virtual Power Plant
- Distributed Energy Resources
- Energy Trading
- Flexibility
- Forecasting
- Grid
---
