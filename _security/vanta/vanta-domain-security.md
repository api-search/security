---
api_specs:
- filename: vanta-openapi.yml
  format: yaml
  label: Vanta API
  slug: vanta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-openapi.yml
- filename: vanta-auditor-openapi.yml
  format: yaml
  label: Vanta Auditor API
  slug: vanta-auditor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-auditor-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vanta.com
  spf: true
hosts:
- cert_expires: Aug 13 16:21:37 2026 GMT
  host: developer.vanta.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api.vanta.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vanta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vanta, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vanta
provider_slug: vanta
slug: vanta-domain-security
source_filename: vanta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.vanta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 16:21:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vanta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vanta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/security/vanta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- Compliance
- Security
- Governance
- Risk Management
---
