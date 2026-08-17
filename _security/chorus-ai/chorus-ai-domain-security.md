---
api_specs:
- filename: chorus-ai-openapi.yml
  format: yaml
  label: Chorus Engagements API
  slug: chorus-engagements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chorus-ai/refs/heads/main/openapi/chorus-ai-openapi.yml
- filename: chorus-ai-openapi.yml
  format: yaml
  label: Chorus Recordings & Transcripts API
  slug: chorus-recordings-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chorus-ai/refs/heads/main/openapi/chorus-ai-openapi.yml
- filename: chorus-ai-openapi.yml
  format: yaml
  label: Chorus CRM Sync API
  slug: chorus-crm-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chorus-ai/refs/heads/main/openapi/chorus-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chorus.ai
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.chorus.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: chorus.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chorus Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chorus.ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chorus.ai
provider_slug: chorus-ai
slug: chorus-ai-domain-security
source_filename: chorus-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chorus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: false\n- host: chorus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: chorus.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chorus-ai/refs/heads/main/security/chorus-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sales
- Revenue Intelligence
- Conversation
- Analytics
- ZoomInfo
- Conversation Intelligence
- Sales Enablement
- Call Recording
- Transcription
- Speech Analytics
- CRM
- Coaching
---
