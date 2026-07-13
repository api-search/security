---
api_specs:
- filename: openapi.json
  format: json
  label: Veritas Volume Manager REST API
  slug: veritas-volume-manager-rest-api
  spec_type: OpenAPI
  url: https://api.veritas.com/vvm/v1/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: veritas.com
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: my.veritas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: www.veritas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.veritas.com
  https: false
kind: domain-security
layout: security
method: probed
name: Veritas Volume Manager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veritas Volume Manager, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Veritas Volume Manager
provider_slug: veritas-volume-manager
slug: veritas-volume-manager-domain-security
source_filename: veritas-volume-manager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: my.veritas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.veritas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.veritas.com\n  https: false\ndomains:\n- domain: veritas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veritas-volume-manager/refs/heads/main/security/veritas-volume-manager-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Disaster Recovery
- Enterprise Storage
- File Systems
- Storage
- Volume Management
---
