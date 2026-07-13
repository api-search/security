---
api_specs:
- filename: lenovo-openapi.yml
  format: yaml
  label: Lenovo XClarity Administrator REST API
  slug: lenovo-xclarity-administrator-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lenovo/refs/heads/main/openapi/lenovo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lenovo.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.lenovo.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: pubs.lenovo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lenovo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lenovo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lenovo
provider_slug: lenovo
slug: lenovo-domain-security
source_filename: lenovo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lenovo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: pubs.lenovo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lenovo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lenovo/refs/heads/main/security/lenovo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Center
- Hardware
- Infrastructure
- Personal Computers
- Servers
- Technology
---
