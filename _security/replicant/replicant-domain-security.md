---
api_specs:
- filename: replicant-outbound-api-openapi.yml
  format: yaml
  label: Replicant Outbound API
  slug: replicant-outbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicant/refs/heads/main/openapi/replicant-outbound-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: replicant.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: replicant.ai
  spf: true
hosts:
- cert_expires: Nov 11 19:29:52 2026 GMT
  host: www.replicant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 03:28:05 2026 GMT
  host: api.replicant.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Replicant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Replicant, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Replicant
provider_slug: replicant
slug: replicant-domain-security
source_filename: replicant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.replicant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 19:29:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.replicant.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 03:28:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: replicant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: replicant.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replicant/refs/heads/main/security/replicant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Contact Center
- Conversational AI
- Customer Service
- Voice AI
- Contact Center Automation
- Agentic AI
- Conversation Intelligence
---
