---
api_specs:
- filename: fyrn-openapi-generated.yml
  format: yaml
  label: Fyrn API
  slug: fyrn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyrn/refs/heads/main/openapi/_ae-authored/fyrn-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fyrn.ai
  spf: true
hosts:
- cert_expires: Jan 15 22:20:36 2027 GMT
  host: fyrn.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fyrn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fyrn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fyrn
provider_slug: fyrn
slug: fyrn-domain-security
source_filename: fyrn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fyrn.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 22:20:36 2027 GMT\n  hsts: false\ndomains:\n- domain: fyrn.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fyrn/refs/heads/main/security/fyrn-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Integration
- AI
- Automation
- Enterprise
- Platform
- Company
---
