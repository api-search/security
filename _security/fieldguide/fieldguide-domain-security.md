---
api_specs:
- filename: fieldguide-openapi-original.json
  format: json
  label: Fieldguide API
  slug: fieldguide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fieldguide.io
  spf: true
hosts:
- cert_expires: Sep  6 14:53:35 2026 GMT
  host: www.fieldguide.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 13:19:33 2026 GMT
  host: api.fieldguide.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fieldguide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fieldguide, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fieldguide
provider_slug: fieldguide
slug: fieldguide-domain-security
source_filename: fieldguide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fieldguide.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 14:53:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fieldguide.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:19:33 2026 GMT\n  hsts: null\ndomains:\n- domain: fieldguide.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/security/fieldguide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Audit
- Advisory
- Accounting
- Compliance
- Risk
- Engagement Management
- Artificial Intelligence
- Agents
- Webhooks
---
