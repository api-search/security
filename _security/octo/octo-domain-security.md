---
api_specs:
- filename: octo-openapi-original.yml
  format: yaml
  label: Open Connectivity for Tours, Activities, and Attractions
  slug: octo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octo/refs/heads/main/openapi/octo-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: octo.travel
  spf: false
hosts:
- cert_expires: Sep 23 13:47:22 2026 GMT
  host: docs.octo.travel
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Octo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Connectivity for Tours, Activities, and Attractions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Open Connectivity for Tours, Activities, and Attractions
provider_slug: octo
slug: octo-domain-security
source_filename: octo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.octo.travel\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 13:47:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: octo.travel\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octo/refs/heads/main/security/octo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Activities
- Attractions
- Open Standard
- Tours
- Travel
---
