---
api_specs:
- filename: velocitycard-cards-api-openapi.yml
  format: yaml
  label: VelocityCard Card Issuing Cards API
  slug: velocitycard-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velocitycard/refs/heads/main/openapi/velocitycard-cards-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: velocitycard.io
  spf: true
hosts:
- cert_expires: Dec 23 18:02:10 2026 GMT
  host: www.velocitycard.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Velocitycard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VelocityCard Card Issuing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VelocityCard Card Issuing
provider_slug: velocitycard
slug: velocitycard-domain-security
source_filename: velocitycard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.velocitycard.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 18:02:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: velocitycard.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/velocitycard/refs/heads/main/security/velocitycard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Card Issuing
- Banking as a Service
- Embedded Finance
- Commercial Cards
- Payments
- Expense Management
---
