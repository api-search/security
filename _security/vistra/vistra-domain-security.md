---
api_specs:
- filename: vistra-incorporations-openapi.yml
  format: yaml
  label: Vistra Incorporations API
  slug: incorporations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vistra/refs/heads/main/openapi/vistra-incorporations-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vistra.com
  spf: true
hosts:
- cert_expires: Oct  8 05:46:36 2026 GMT
  host: www.vistra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 08:20:16 2026 GMT
  host: help.vistra.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: api.vistra.com
  https: false
kind: domain-security
layout: security
method: probed
name: Vistra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vistra, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vistra
provider_slug: vistra
slug: vistra-domain-security
source_filename: vistra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vistra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:46:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.vistra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:20:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.vistra.com\n  https: false\ndomains:\n- domain: vistra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vistra/refs/heads/main/security/vistra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compliance
- Corporate Services
- Entity Management
- Finance
- Fortune 500
- Legal
---
