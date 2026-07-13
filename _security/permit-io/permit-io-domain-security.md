---
api_specs:
- filename: permit-io-openapi.json
  format: json
  label: Permit.io API
  slug: permit-io
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permit-io/refs/heads/main/openapi/permit-io-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: permit.io
  spf: true
hosts:
- cert_expires: Aug 22 03:54:00 2026 GMT
  host: www.permit.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 23:43:44 2026 GMT
  host: docs.permit.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: api.permit.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Permit Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Permit.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Permit.io
provider_slug: permit-io
slug: permit-io-domain-security
source_filename: permit-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.permit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 03:54:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.permit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 23:43:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.permit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: permit.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/permit-io/refs/heads/main/security/permit-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Access Control
- Authorization
- Identity
- Policy
- Security
---
