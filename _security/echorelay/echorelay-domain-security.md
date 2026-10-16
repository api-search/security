---
api_specs:
- filename: echorelay-openapi-generated.yml
  format: yaml
  label: EchoRelay API
  slug: echorelay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/echorelay/refs/heads/main/openapi/_ae-authored/echorelay-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: echorelay.dev
  spf: true
hosts:
- cert_expires: Dec 11 09:46:42 2026 GMT
  host: echorelay.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Echorelay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EchoRelay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: EchoRelay
provider_slug: echorelay
slug: echorelay-domain-security
source_filename: echorelay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: echorelay.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 09:46:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: echorelay.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echorelay/refs/heads/main/security/echorelay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API
- Integration
- Platform
- Automation
- NoCode
- Company
---
