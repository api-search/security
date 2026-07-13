---
api_specs:
- filename: polyapi-platform-openapi.yml
  format: yaml
  label: PolyAPI Platform API
  slug: polyapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/openapi/polyapi-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: polyapi.io
  spf: true
hosts:
- cert_expires: Aug 29 03:32:33 2026 GMT
  host: polyapi.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 03:25:02 2026 GMT
  host: na1.polyapi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 06:37:32 2026 GMT
  host: eu1.polyapi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polyapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PolyAPI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PolyAPI
provider_slug: polyapi
slug: polyapi-domain-security
source_filename: polyapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polyapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 03:32:33 2026 GMT\n  hsts: false\n- host: na1.polyapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 03:25:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eu1.polyapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:37:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: polyapi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/security/polyapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Integrations
- Microservices
- Middleware
- Orchestrations
- Pro-Code API Composition
---
