---
api_specs:
- filename: contrast-security-openapi.yml
  format: yaml
  label: Contrast TeamServer REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contrast-security/refs/heads/main/openapi/contrast-security-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: contrastsecurity.com
  spf: true
hosts:
- cert_expires: Sep 21 19:02:51 2026 GMT
  host: www.contrastsecurity.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 17:00:26 2026 GMT
  host: api.contrastsecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 17:00:26 2026 GMT
  host: app.contrastsecurity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Contrast Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contrast Security, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Contrast Security
provider_slug: contrast-security
slug: contrast-security-domain-security
source_filename: contrast-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.contrastsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:02:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.contrastsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 17:00:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.contrastsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 17:00:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: contrastsecurity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contrast-security/refs/heads/main/security/contrast-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Application Security
- AppSec
- IAST
- RASP
- SCA
- DevSecOps
- Runtime Protection
---
