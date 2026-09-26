---
api_specs:
- filename: tohuman-openapi-generated.yml
  format: yaml
  label: ToHuman API
  slug: tohuman-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tohuman/refs/heads/main/openapi/_ae-authored/tohuman-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tohuman.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: astral.sh
  spf: true
hosts:
- cert_expires: Dec 15 21:37:03 2026 GMT
  host: tohuman.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 20:45:53 2026 GMT
  host: astral.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Tohuman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ToHuman, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ToHuman
provider_slug: tohuman
slug: tohuman-domain-security
source_filename: tohuman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tohuman.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 21:37:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: astral.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 20:45:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tohuman.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: astral.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tohuman/refs/heads/main/security/tohuman-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Text-Humanization
- Content-Generation
- Marketing
- SaaS
---
