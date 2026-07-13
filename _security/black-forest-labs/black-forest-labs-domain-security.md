---
api_specs:
- filename: black-forest-labs-openapi.yml
  format: yaml
  label: Flux Image Generation API
  slug: flux
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/black-forest-labs/refs/heads/main/openapi/black-forest-labs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blackforestlabs.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bfl.ai
  spf: false
hosts:
- cert_expires: Aug 12 09:18:59 2026 GMT
  host: blackforestlabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.bfl.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: api.bfl.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Black Forest Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Black Forest Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Black Forest Labs
provider_slug: black-forest-labs
slug: black-forest-labs-domain-security
source_filename: black-forest-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blackforestlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 09:18:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.bfl.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.bfl.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blackforestlabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bfl.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-forest-labs/refs/heads/main/security/black-forest-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Image Generation
- Flux
- Open Weights
- BFL
---
