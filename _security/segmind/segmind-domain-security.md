---
api_specs:
- filename: segmind-openapi.yml
  format: yaml
  label: Segmind
  slug: segmind
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/openapi/segmind-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: segmind.com
  spf: true
hosts:
- cert_expires: Sep 21 01:30:14 2026 GMT
  host: www.segmind.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: api.segmind.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: workflows-api.segmind.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Segmind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Segmind, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Segmind
provider_slug: segmind
slug: segmind-domain-security
source_filename: segmind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.segmind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 01:30:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.segmind.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\n- host: workflows-api.segmind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: segmind.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/security/segmind-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
