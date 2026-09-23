---
api_specs:
- filename: accor-openapi-generated.yml
  format: yaml
  label: Accor API
  slug: accor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/openapi/_ae-authored/accor-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: accor.com
  spf: true
hosts:
- cert_expires: Nov 25 07:33:13 2026 GMT
  host: accor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Accor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Accor
provider_slug: accor
slug: accor-domain-security
source_filename: accor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: accor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 07:33:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: accor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accor/refs/heads/main/security/accor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hospitality
- Travel
- Hotels
- Technology
---
