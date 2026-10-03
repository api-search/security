---
api_specs:
- filename: proof-random-api-random-api-openapi.yml
  format: yaml
  label: Proof Random API (Kepler Ops) Random API
  slug: proof-random-api-random-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proof-random-api/refs/heads/main/openapi/proof-random-api-random-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workers.dev
  spf: true
hosts:
- cert_expires: Dec 13 17:10:25 2026 GMT
  host: proof-random-api.pn-26f.workers.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Proof Random Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proof Random API (Kepler Ops), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Proof Random API (Kepler Ops)
provider_slug: proof-random-api
slug: proof-random-api-domain-security
source_filename: proof-random-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: proof-random-api.pn-26f.workers.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 17:10:25 2026 GMT\n  hsts: false\ndomains:\n- domain: workers.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proof-random-api/refs/heads/main/security/proof-random-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Randomness
- Public APIs
- Drand
- Free Service
---
