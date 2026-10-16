---
api_specs:
- filename: api7-openapi-generated.yml
  format: yaml
  label: API7.ai API
  slug: api7-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api7/refs/heads/main/openapi/_ae-authored/api7-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: api7.ai
  spf: true
hosts:
- cert_expires: Nov 20 01:45:43 2026 GMT
  host: api7.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Api7 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API7.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: API7.ai
provider_slug: api7
slug: api7-domain-security
source_filename: api7-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api7.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 01:45:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: api7.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api7/refs/heads/main/security/api7-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API Gateway
- AI Gateway
- Open Source
- Cloud
---
