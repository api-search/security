---
api_specs:
- filename: fetchlayer-openapi-generated.yml
  format: yaml
  label: HootCodes API
  slug: fetchlayer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fetchlayer/refs/heads/main/openapi/_ae-authored/fetchlayer-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fetchlayer.dev
  spf: true
hosts:
- cert_expires: Dec  8 18:49:38 2026 GMT
  host: fetchlayer.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fetchlayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HootCodes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HootCodes
provider_slug: fetchlayer
slug: fetchlayer-domain-security
source_filename: fetchlayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fetchlayer.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 18:49:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fetchlayer.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fetchlayer/refs/heads/main/security/fetchlayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social Media
- Data Extraction
- API
- SaaS
---
