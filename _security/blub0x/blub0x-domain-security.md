---
api_specs:
- filename: blub0x-openapi-generated.yml
  format: yaml
  label: Blub0x API
  slug: blub0x-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blub0x/refs/heads/main/openapi/_ae-authored/blub0x-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blub0x.com
  spf: true
hosts:
- cert_expires: Dec 12 23:30:29 2026 GMT
  host: www.blub0x.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blub0X Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blub0x, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Blub0x
provider_slug: blub0x
slug: blub0x-domain-security
source_filename: blub0x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blub0x.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:30:29 2026 GMT\n  hsts: false\ndomains:\n- domain: blub0x.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blub0x/refs/heads/main/security/blub0x-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Physical Security
- Cloud Security
- Access Control
- Elevator Management
- AI
---
