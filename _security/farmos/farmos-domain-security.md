---
api_specs:
- filename: farmos-farmos-api-openapi.yml
  format: yaml
  label: farmOS JSON:API
  slug: farmos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmos/refs/heads/main/openapi/farmos-farmos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: farmos.org
  spf: true
hosts:
- cert_expires: Sep 20 19:53:58 2026 GMT
  host: farmos.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Farmos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for farmOS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: farmOS
provider_slug: farmos
slug: farmos-domain-security
source_filename: farmos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: farmos.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:53:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: farmos.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmos/refs/heads/main/security/farmos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- Farm Management
- Open Source
- JSON:API
- Record Keeping
- Self-Hosted
- Drupal
---
