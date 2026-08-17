---
api_specs:
- filename: dashbot-export-api-openapi.yml
  format: yaml
  label: Dashbot Export API
  slug: dashbot-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dashbot/refs/heads/main/openapi/dashbot-export-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dimensionlabs.io
  spf: true
hosts:
- cert_expires: Oct 15 10:24:12 2026 GMT
  host: www.dimensionlabs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 22:29:24 2026 GMT
  host: docs.dimensionlabs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.dimensionlabs.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dashbot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dashbot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dashbot
provider_slug: dashbot
slug: dashbot-domain-security
source_filename: dashbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dimensionlabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 10:24:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dimensionlabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:29:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dimensionlabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dimensionlabs.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dashbot/refs/heads/main/security/dashbot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Conversational Analytics
- Chatbots
- Voice Assistants
- Customer Experience
- Data Enrichment
- Analytics
- Contact Center
---
