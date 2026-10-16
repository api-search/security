---
api_specs:
- filename: fused-openapi-generated.yml
  format: yaml
  label: Fused API
  slug: fused-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fused/refs/heads/main/openapi/_ae-authored/fused-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fused.io
  spf: true
hosts:
- cert_expires: Dec 11 18:22:07 2026 GMT
  host: www.fused.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fused Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fused, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fused
provider_slug: fused
slug: fused-domain-security
source_filename: fused-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fused.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 18:22:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fused.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fused/refs/heads/main/security/fused-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Analytics
- AI
- DataPlatform
- Python
- LowCode
---
