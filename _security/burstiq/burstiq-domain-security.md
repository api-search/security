---
api_specs:
- filename: burstiq-lifegraph-openapi-original.json
  format: json
  label: BurstIQ LifeGraph API
  slug: burstiq-lifegraph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burstiq/refs/heads/main/openapi/burstiq-lifegraph-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: burstiq.com
  spf: true
hosts:
- cert_expires: Oct  4 07:20:51 2026 GMT
  host: burstiq.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Burstiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BurstIQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BurstIQ
provider_slug: burstiq
slug: burstiq-domain-security
source_filename: burstiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: burstiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:20:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: burstiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/burstiq/refs/heads/main/security/burstiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Data
- Blockchain
- Knowledge Graph
- Consent
- Agentic AI
---
