---
api_specs:
- filename: nuira-ai-openapi-generated.yml
  format: yaml
  label: Nuira API
  slug: nuira-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuira-ai/openapi/_ae-authored/nuira-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nuira.ai
  spf: true
hosts:
- cert_expires: Dec 23 06:36:48 2026 GMT
  host: nuira.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nuira Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuira, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nuira
provider_slug: nuira-ai
slug: nuira-ai-domain-security
source_filename: nuira-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nuira.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 06:36:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nuira.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/nuira-ai/security/nuira-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Artificial Intelligence
- Analytics
- Profit
---
