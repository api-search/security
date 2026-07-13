---
api_specs:
- filename: fastdol-openapi.yml
  format: yaml
  label: FastDOL API
  slug: fastdol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastdol/main/openapi/fastdol-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fastdol.com
  spf: true
hosts:
- cert_expires: Sep  4 10:45:37 2026 GMT
  host: fastdol.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 11:54:49 2026 GMT
  host: api.fastdol.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fastdol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FastDOL, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FastDOL
provider_slug: fastdol
slug: fastdol-domain-security
source_filename: fastdol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fastdol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 10:45:37 2026 GMT\n  hsts: null\n- host: api.fastdol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 11:54:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fastdol.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastdol/refs/heads/main/security/fastdol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- OSHA
- Compliance
- Workplace Safety
- Public Records
- Federal Enforcement
- Labor
---
