---
api_specs:
- filename: citoapi-v1-openapi.json
  format: json
  label: Cito API V1 API
  slug: cito-api-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citoapi/refs/heads/main/openapi/_original/citoapi-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: citoapi.com
  spf: true
hosts:
- cert_expires: Dec  1 00:55:56 2026 GMT
  host: citoapi.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Citoapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cito CS2 API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cito CS2 API
provider_slug: citoapi
slug: citoapi-domain-security
source_filename: citoapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: citoapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 00:55:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: citoapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citoapi/refs/heads/main/security/citoapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API
- Esports
- Gaming
- Data
---
