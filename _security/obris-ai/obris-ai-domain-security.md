---
api_specs:
- filename: obris-ai-openapi-generated.yml
  format: yaml
  label: Obris API
  slug: obris-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obris-ai/openapi/_ae-authored/obris-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: obris.ai
  spf: false
hosts:
- cert_expires: Jan 12 19:49:55 2027 GMT
  host: obris.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Obris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Obris, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Obris
provider_slug: obris-ai
slug: obris-ai-domain-security
source_filename: obris-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: obris.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 19:49:55 2027 GMT\n  hsts: false\ndomains:\n- domain: obris.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/obris-ai/security/obris-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Knowledge Management
- Productivity
- Collaboration
- Platform
---
