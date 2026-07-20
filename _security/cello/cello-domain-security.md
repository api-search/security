---
api_specs:
- filename: cello-openapi-original.json
  format: json
  label: Cello API
  slug: cello-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cello.so
  spf: true
hosts:
- cert_expires: Oct  1 11:33:35 2026 GMT
  host: docs.cello.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: api.cello.so
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: api.sandbox.cello.so
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cello Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cello, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cello
provider_slug: cello
slug: cello-domain-security
source_filename: cello-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.cello.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:33:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cello.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: api.sandbox.cello.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cello.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/security/cello-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Referral Marketing
- Affiliate Marketing
- Growth
- SaaS
- Attribution
- Partner Programs
- Ai Enterprise Software
---
