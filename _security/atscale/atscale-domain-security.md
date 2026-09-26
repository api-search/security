---
api_specs:
- filename: atscale-openapi-generated.yml
  format: yaml
  label: Atscale API
  slug: atscale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atscale/refs/heads/main/openapi/_ae-authored/atscale-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atscale.com
  spf: true
hosts:
- cert_expires: Nov 28 10:15:38 2026 GMT
  host: www.atscale.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atscale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atscale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atscale
provider_slug: atscale
slug: atscale-domain-security
source_filename: atscale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 10:15:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atscale.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atscale/refs/heads/main/security/atscale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Business Intelligence
- Data Integration
- AI
- Semantic Layer
---
