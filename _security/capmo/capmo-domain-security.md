---
api_specs:
- filename: capmo-rest-api-openapi-original.json
  format: json
  label: Capmo REST API
  slug: capmo-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capmo/refs/heads/main/openapi/capmo-rest-api-openapi-original.json
- filename: capmo-webhook-api-openapi-original.json
  format: json
  label: Capmo Webhook API
  slug: capmo-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capmo/refs/heads/main/openapi/capmo-webhook-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: capmo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: capmo.de
  spf: true
hosts:
- cert_expires: Sep 28 05:19:18 2026 GMT
  host: www.capmo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: api.capmo.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capmo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capmo, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Capmo
provider_slug: capmo
slug: capmo-domain-security
source_filename: capmo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.capmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:19:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.capmo.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: capmo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: capmo.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capmo/refs/heads/main/security/capmo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Vertical Software
- Construction
- Project Management
- Construction Tech
- Field Management
- Building
- DACH
---
