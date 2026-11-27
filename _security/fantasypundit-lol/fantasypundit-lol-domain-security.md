---
api_specs:
- filename: fantasypundit-lol-calendar-api-openapi.yml
  format: yaml
  label: Fantasy Pundit Calendar API
  slug: fantasypundit-lol-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fantasypundit-lol/openapi/fantasypundit-lol-calendar-api-openapi.yml
- filename: fantasypundit-lol-commentary-api-openapi.yml
  format: yaml
  label: Fantasy Pundit Commentary API
  slug: fantasypundit-lol-commentary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fantasypundit-lol/openapi/fantasypundit-lol-commentary-api-openapi.yml
- filename: fantasypundit-lol-status-api-openapi.yml
  format: yaml
  label: Fantasy Pundit Status API
  slug: fantasypundit-lol-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fantasypundit-lol/openapi/fantasypundit-lol-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fantasypundit.lol
  spf: true
hosts:
- cert_expires: Dec 29 08:58:56 2026 GMT
  host: fantasypundit.lol
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fantasy Pundit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fantasy Pundit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fantasy Pundit
provider_slug: fantasypundit-lol
slug: fantasypundit-lol-domain-security
source_filename: fantasypundit-lol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fantasypundit.lol\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 08:58:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fantasypundit.lol\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fantasypundit-lol/security/fantasypundit-lol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
---
