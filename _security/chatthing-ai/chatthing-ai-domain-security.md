---
api_specs:
- filename: chatthing-ai-openapi-generated.yml
  format: yaml
  label: Chat Thing API
  slug: chatthing-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatthing-ai/openapi/_ae-authored/chatthing-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: chatthing.ai
  spf: true
hosts:
- cert_expires: Jan 17 18:50:09 2027 GMT
  host: chatthing.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chatthing Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chat Thing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Chat Thing
provider_slug: chatthing-ai
slug: chatthing-ai-domain-security
source_filename: chatthing-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chatthing.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 18:50:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chatthing.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/chatthing-ai/security/chatthing-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Chatbot
- Customer Service
- Lead Capture
- Appointment Booking
- Voice Assistant
- Internal knowledge base
- SDK
---
