---
api_specs:
- filename: termscout-contract-positions-api-openapi.yml
  format: yaml
  label: TermScout Contract Positions API
  slug: termscout-contract-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termscout/refs/heads/main/openapi/termscout-contract-positions-api-openapi.yml
- filename: termscout-contracts-api-openapi.yml
  format: yaml
  label: TermScout Contracts API
  slug: termscout-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termscout/refs/heads/main/openapi/termscout-contracts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: termscout.com
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: termscout.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: api.termscout.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Termscout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TermScout, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TermScout
provider_slug: termscout
slug: termscout-domain-security
source_filename: termscout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: termscout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.termscout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: termscout.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/termscout/refs/heads/main/security/termscout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legal Tech
- Contract Intelligence
- Contract Certification
- Contract Analysis
- Procurement
- Legal Operations
- Sales Enablement
- Artificial Intelligence
- Contract Data
- Document Analysis
---
