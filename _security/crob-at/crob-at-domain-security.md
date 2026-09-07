---
api_specs:
- filename: crob-at-openapi.json
  format: json
  label: crob.at REST API
  slug: crobat-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crob-at/refs/heads/main/openapi/crob-at-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crob.at
  spf: true
hosts:
- cert_expires: Nov 16 15:00:56 2026 GMT
  host: crob.at
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crob At Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for crob.at, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: crob.at
provider_slug: crob-at
slug: crob-at-domain-security
source_filename: crob-at-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crob.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 15:00:56 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: crob.at\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crob-at/refs/heads/main/security/crob-at-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gaming
- Esports
- Pokemon
- Pokemon Showdown
- Team Building
- Content Rendering
- Developer Tools
- REST API
---
