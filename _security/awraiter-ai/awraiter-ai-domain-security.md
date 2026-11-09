---
api_specs:
- filename: awraiter-ai-catalog-api-openapi.yml
  format: yaml
  label: AwrAiter Catalog API
  slug: awraiter-ai-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awraiter-ai/openapi/awraiter-ai-catalog-api-openapi.yml
- filename: awraiter-ai-read-api-openapi.yml
  format: yaml
  label: AwrAiter Read API
  slug: awraiter-ai-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awraiter-ai/openapi/awraiter-ai-read-api-openapi.yml
- filename: awraiter-ai-write-api-openapi.yml
  format: yaml
  label: AwrAiter Write API
  slug: awraiter-ai-write-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awraiter-ai/openapi/awraiter-ai-write-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: awraiter.ai
  spf: false
hosts:
- cert_expires: Dec 31 09:49:26 2026 GMT
  host: awraiter.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Awraiter Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AwrAiter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: AwrAiter
provider_slug: awraiter-ai
slug: awraiter-ai-domain-security
source_filename: awraiter-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: awraiter.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 09:49:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: awraiter.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/awraiter-ai/security/awraiter-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telegram
- Content Planning
- Analytics
- AI Integration
- Software-as-a-Service
---
