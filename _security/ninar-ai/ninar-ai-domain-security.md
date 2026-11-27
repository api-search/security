---
api_specs:
- filename: ninar-ai-crm-api-openapi.yml
  format: yaml
  label: Ninar AI CRM API
  slug: ninar-ai-crm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ninar-ai/openapi/ninar-ai-crm-api-openapi.yml
- filename: ninar-ai-visibility-api-openapi.yml
  format: yaml
  label: Ninar AI Visibility API
  slug: ninar-ai-visibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ninar-ai/openapi/ninar-ai-visibility-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ninar.ai
  spf: true
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: ninar.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ninar AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ninar AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ninar AI
provider_slug: ninar-ai
slug: ninar-ai-domain-security
source_filename: ninar-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ninar.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ninar.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ninar-ai/security/ninar-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Marketing
- Analytics
- Brand Visibility
- Software-as-a-Service
---
