---
api_specs:
- filename: magier-openapi-generated.yml
  format: yaml
  label: Magier AI API
  slug: magier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magier/refs/heads/main/openapi/_ae-authored/magier-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: magier.ai
  spf: false
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: magier.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Magier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magier AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Magier AI
provider_slug: magier
slug: magier-domain-security
source_filename: magier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magier.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: magier.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magier/refs/heads/main/security/magier-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Cybersecurity
- Compliance
- Governance
---
