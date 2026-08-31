---
api_specs:
- filename: voygr-calls-api-openapi.yml
  format: yaml
  label: Voygr Calls API
  slug: voygr-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voygr/refs/heads/main/openapi/voygr-calls-api-openapi.yml
- filename: voygr-core-api-openapi.yml
  format: yaml
  label: VOYGR Core API
  slug: voygr-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voygr/refs/heads/main/openapi/voygr-core-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: voygr.tech
  spf: true
hosts:
- cert_expires: Oct 24 07:17:56 2026 GMT
  host: voygr.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: api.voygr.tech
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Voygr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VOYGR, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VOYGR
provider_slug: voygr
slug: voygr-domain-security
source_filename: voygr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voygr.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 07:17:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.voygr.tech\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: voygr.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voygr/refs/heads/main/security/voygr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Location Intelligence
- POI Data
- Data Enrichment
- Data Validation
- Geospatial
- Places
- AI Agents
- Agent Skills
- Voice AI
- Telephony
- Outbound Calls
- Business Validation
- Y Combinator
---
