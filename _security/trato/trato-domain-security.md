---
api_specs:
- filename: trato-openapi.yml
  format: yaml
  label: TRATO Contract API
  slug: trato-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trato/refs/heads/main/openapi/trato-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trato.io
  spf: true
hosts:
- cert_expires: Sep  7 10:58:15 2026 GMT
  host: trato.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trato, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Trato
provider_slug: trato
slug: trato-domain-security
source_filename: trato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trato.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 10:58:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trato.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trato/refs/heads/main/security/trato-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Contract Management
- Contract Lifecycle Management
- Electronic Signature
- Legaltech
- Document Management
- Workflow Automation
- Legal
---
