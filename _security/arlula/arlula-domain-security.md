---
api_specs:
- filename: arlula-openapi.yaml
  format: yaml
  label: Arlula API
  slug: arlula-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/openapi/arlula-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arlula.com
  spf: true
hosts:
- cert_expires: Sep 29 05:42:36 2026 GMT
  host: arlula.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 23:48:34 2026 GMT
  host: dashboard.arlula.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 23:48:48 2026 GMT
  host: api.arlula.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arlula Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arlula, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arlula
provider_slug: arlula
slug: arlula-domain-security
source_filename: arlula-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arlula.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:42:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dashboard.arlula.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:48:34 2026 GMT\n  hsts: null\n- host: api.arlula.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:48:48 2026 GMT\n  hsts: null\ndomains:\n- domain: arlula.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/security/arlula-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
---
