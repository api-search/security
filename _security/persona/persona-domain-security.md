---
api_specs:
- filename: persona-openapi.yml
  format: yaml
  label: Persona API
  slug: persona
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: withpersona.com
  spf: true
hosts:
- cert_expires: Aug 23 00:29:30 2026 GMT
  host: withpersona.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 01:41:23 2026 GMT
  host: docs.withpersona.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Persona Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Persona, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Persona
provider_slug: persona
slug: persona-domain-security
source_filename: persona-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: withpersona.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 00:29:30 2026 GMT\n  hsts: null\n- host: docs.withpersona.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:41:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: withpersona.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/security/persona-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Prevention
- Identity Verification
- KYC
---
