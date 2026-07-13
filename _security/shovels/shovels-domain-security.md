---
api_specs:
- filename: shovels-openapi.yml
  format: yaml
  label: Shovels API
  slug: shovels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shovels/refs/heads/main/openapi/shovels-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shovels.ai
  spf: true
hosts:
- cert_expires: Sep 29 01:19:22 2026 GMT
  host: www.shovels.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: api.shovels.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shovels Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shovels, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shovels
provider_slug: shovels
slug: shovels-domain-security
source_filename: shovels-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shovels.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 01:19:22 2026 GMT\n  hsts: false\n- host: api.shovels.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: shovels.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shovels/refs/heads/main/security/shovels-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Construction
- Building Permits
- Contractors
- Real Estate
- Property Data
- Market Intelligence
---
