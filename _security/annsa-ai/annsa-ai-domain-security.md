---
api_specs:
- filename: annsa-ai-agents-api-openapi.yml
  format: yaml
  label: Annsa Agents API
  slug: annsa-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/annsa-ai/openapi/annsa-ai-agents-api-openapi.yml
- filename: annsa-ai-ingest-api-openapi.yml
  format: yaml
  label: Annsa Ingest API
  slug: annsa-ai-ingest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/annsa-ai/openapi/annsa-ai-ingest-api-openapi.yml
- filename: annsa-ai-service-api-openapi.yml
  format: yaml
  label: Annsa Service API
  slug: annsa-ai-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/annsa-ai/openapi/annsa-ai-service-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: annsa.ai
  spf: false
hosts:
- cert_expires: Jan 23 01:21:50 2027 GMT
  host: annsa.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Annsa Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Annsa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Annsa
provider_slug: annsa-ai
slug: annsa-ai-domain-security
source_filename: annsa-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: annsa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 01:21:50 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: annsa.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/annsa-ai/security/annsa-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Project Management
- Customer Management
- Agent Teams
- Artificial Intelligence
- Software-as-a-Service
---
