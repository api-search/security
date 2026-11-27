---
api_specs:
- filename: okibi-ai-openapi-generated.yml
  format: yaml
  label: Okibi API
  slug: okibi-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/okibi-ai/openapi/_ae-authored/okibi-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: okibi.ai
  spf: true
hosts:
- cert_expires: Feb 14 23:35:39 2027 GMT
  host: okibi.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Okibi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Okibi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Okibi
provider_slug: okibi-ai
slug: okibi-ai-domain-security
source_filename: okibi-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: okibi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:35:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: okibi.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/okibi-ai/security/okibi-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- CLI
- Automation
- Agents
- Platform
---
