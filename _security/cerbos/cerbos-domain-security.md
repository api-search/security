---
api_specs:
- filename: swagger.json
  format: json
  label: Cerbos PDP REST API
  slug: cerbos-pdp-rest-api
  spec_type: OpenAPI
  url: https://docs.cerbos.dev/cerbos/latest/api/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cerbos.dev
  spf: true
hosts:
- cert_expires: Sep 13 23:10:33 2026 GMT
  host: www.cerbos.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 11:43:42 2026 GMT
  host: docs.cerbos.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cerbos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cerbos, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cerbos
provider_slug: cerbos
slug: cerbos-domain-security
source_filename: cerbos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cerbos.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:10:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.cerbos.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 11:43:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cerbos.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerbos/refs/heads/main/security/cerbos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- ABAC
- Access Control
- Authorization
- AuthZEN
- Open Source
- PBAC
- PDP
- Permissions
- Policy as Code
- RBAC
- ReBAC
- Zero Trust
---
