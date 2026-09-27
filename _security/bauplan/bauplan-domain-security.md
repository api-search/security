---
api_specs:
- filename: bauplan-openapi-generated.yml
  format: yaml
  label: Bauplan API
  slug: bauplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bauplan/refs/heads/main/openapi/_ae-authored/bauplan-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bauplanlabs.com
  spf: true
hosts:
- cert_expires: Nov 13 20:33:58 2026 GMT
  host: bauplanlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bauplan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bauplan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bauplan
provider_slug: bauplan
slug: bauplan-domain-security
source_filename: bauplan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bauplanlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 20:33:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bauplanlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bauplan/refs/heads/main/security/bauplan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Engineering
- AI Agents
- Serverless Platform
- Data Pipelines
- Data Integration
- Isolation and Rollback
---
