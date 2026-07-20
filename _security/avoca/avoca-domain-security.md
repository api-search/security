---
api_specs:
- filename: avoca-openapi-original.json
  format: json
  label: Avoca Enterprise API
  slug: avoca-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avoca.ai
  spf: true
hosts:
- cert_expires: Oct 15 22:14:12 2026 GMT
  host: docs.avoca.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 11:09:40 2026 GMT
  host: enterprise-api.avoca.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avoca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avoca, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Avoca
provider_slug: avoca
slug: avoca-domain-security
source_filename: avoca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.avoca.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 22:14:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: enterprise-api.avoca.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 11:09:40 2026 GMT\n  hsts: null\ndomains:\n- domain: avoca.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/security/avoca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Voice AI
- Conversational AI
- Customer Service
- Contact Center
- Home Services
- Field Service
- Scheduling
- Analytics
- Webhooks
- Enterprise API
---
