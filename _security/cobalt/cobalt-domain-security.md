---
api_specs:
- filename: cobalt-api-openapi.yml
  format: yaml
  label: Cobalt API
  slug: cobalt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/openapi/cobalt-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gocobalt.io
  spf: true
hosts:
- cert_expires: Oct  4 09:57:47 2026 GMT
  host: www.gocobalt.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: docs.gocobalt.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 04:08:51 2026 GMT
  host: api.gocobalt.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cobalt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cobalt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cobalt
provider_slug: cobalt
slug: cobalt-domain-security
source_filename: cobalt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gocobalt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 09:57:47 2026 GMT\n  hsts: false\n- host: docs.gocobalt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gocobalt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 04:08:51 2026 GMT\n  hsts: null\ndomains:\n- domain: gocobalt.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/security/cobalt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Embedded iPaaS
- Integrations
---
