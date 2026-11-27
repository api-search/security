---
api_specs:
- filename: akkrudata-ai-openapi-generated.yml
  format: yaml
  label: AkkruData API
  slug: akkrudata-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/akkrudata-ai/openapi/_ae-authored/akkrudata-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: akkrudata.ai
  spf: true
hosts:
- cert_expires: Jan 13 14:47:10 2027 GMT
  host: akkrudata.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AkkruData Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AkkruData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: AkkruData
provider_slug: akkrudata-ai
slug: akkrudata-ai-domain-security
source_filename: akkrudata-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: akkrudata.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 14:47:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: akkrudata.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/akkrudata-ai/security/akkrudata-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Data
- Artificial Intelligence
- Filings
---
