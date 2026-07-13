---
api_specs:
- filename: hotjar-rest-api-openapi.yml
  format: yaml
  label: Hotjar REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotjar/refs/heads/main/openapi/hotjar-rest-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hotjar.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: hotjar.io
  spf: true
hosts:
- cert_expires: Sep 16 23:40:11 2026 GMT
  host: help.hotjar.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- host: api.hotjar.com
  https: false
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.hotjar.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hotjar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hotjar, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: hotjar
provider_slug: hotjar
slug: hotjar-domain-security
source_filename: hotjar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: help.hotjar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:40:11 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.hotjar.com\n  https: false\n- host: api.hotjar.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hotjar.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hotjar.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotjar/refs/heads/main/security/hotjar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
