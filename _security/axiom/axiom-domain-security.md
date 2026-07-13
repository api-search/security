---
api_specs:
- filename: axiom-openapi.yml
  format: yaml
  label: Axiom API
  slug: axiom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: axiom.co
  spf: true
hosts:
- cert_expires: Sep 18 23:30:49 2026 GMT
  host: axiom.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: api.axiom.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axiom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axiom, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Axiom
provider_slug: axiom
slug: axiom-domain-security
source_filename: axiom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axiom.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:30:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.axiom.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: axiom.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/security/axiom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Log Management
- Logging
- Observability
- Real-Time
- Serverless
---
