---
api_specs:
- filename: bluebeam-studio-openapi.yml
  format: yaml
  label: Bluebeam Studio API
  slug: bluebeam-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluebeam/refs/heads/main/openapi/bluebeam-studio-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bluebeam.com
  spf: true
hosts:
- cert_expires: Sep 16 01:28:32 2026 GMT
  host: www.bluebeam.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: developers.bluebeam.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api.bluebeam.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bluebeam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bluebeam, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: bluebeam
provider_slug: bluebeam
slug: bluebeam-domain-security
source_filename: bluebeam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bluebeam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:28:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.bluebeam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: false\n- host: api.bluebeam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bluebeam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluebeam/refs/heads/main/security/bluebeam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
