---
api_specs:
- filename: getoya-ai-openapi-generated.yml
  format: yaml
  label: OYA AI Inc. API
  slug: getoya-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getoya-ai/openapi/_ae-authored/getoya-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getoya.ai
  spf: true
hosts:
- cert_expires: Dec 12 03:17:52 2026 GMT
  host: getoya.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OYA AI Inc. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OYA AI Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OYA AI Inc.
provider_slug: getoya-ai
slug: getoya-ai-domain-security
source_filename: getoya-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getoya.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 03:17:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getoya.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getoya-ai/security/getoya-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Automation
- Platform
- Agents
---
