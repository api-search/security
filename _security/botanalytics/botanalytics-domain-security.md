---
api_specs:
- filename: botanalytics-messages-openapi.yml
  format: yaml
  label: Botanalytics Message Ingestion API
  slug: botanalytics-message-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botanalytics/refs/heads/main/openapi/botanalytics-messages-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: botanalytics.co
  spf: false
hosts:
- cert_expires: Aug 28 15:13:52 2026 GMT
  host: botanalytics.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Botanalytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Botanalytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Botanalytics
provider_slug: botanalytics
slug: botanalytics-domain-security
source_filename: botanalytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: botanalytics.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 15:13:52 2026 GMT\n  hsts: false\ndomains:\n- domain: botanalytics.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botanalytics/refs/heads/main/security/botanalytics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Conversational Analytics
- Chatbots
- Voice Assistants
- Bot Analytics
- Analytics
- Natural Language Understanding
- Developer Tools
---
