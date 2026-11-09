---
api_specs:
- filename: dooza-ai-v1-openapi.json
  format: json
  label: Dooza Crew Task API V1 API
  slug: dooza-crew-task-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dooza-ai/openapi/_original/dooza-ai-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dooza.ai
  spf: true
hosts:
- cert_expires: Feb  3 18:07:52 2027 GMT
  host: dooza.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dooza Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dooza, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dooza
provider_slug: dooza-ai
slug: dooza-ai-domain-security
source_filename: dooza-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dooza.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 18:07:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dooza.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dooza-ai/security/dooza-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Employees
- Automation
- Customer Service
- Insurance
- Trucking
- Legal
- Medical Billing
---
