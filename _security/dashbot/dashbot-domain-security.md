---
api_specs:
- filename: dashbot-export-openapi.json
  format: json
  label: Dashbot / Dimension Labs Export API
  slug: dashbot-dimension-labs-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dashbot/refs/heads/main/openapi/dashbot-export-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dashbot.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dimensionlabs.io
  spf: true
hosts:
- cert_expires: Aug 19 23:02:28 2026 GMT
  host: www.dashbot.io
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
overview: 'Domain security posture for Dashbot, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dashbot
provider_slug: dashbot
slug: dashbot-domain-security
source_filename: dashbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dashbot.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:02:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dimensionlabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dashbot.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: dimensionlabs.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
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
