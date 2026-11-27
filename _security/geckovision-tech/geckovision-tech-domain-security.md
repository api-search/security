---
api_specs:
- filename: geckovision-tech-case-studies-api-openapi.yml
  format: yaml
  label: Gecko Case Studies API
  slug: geckovision-tech-case-studies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geckovision-tech/openapi/geckovision-tech-case-studies-api-openapi.yml
- filename: geckovision-tech-waitlist-api-openapi.yml
  format: yaml
  label: Gecko Waitlist API
  slug: geckovision-tech-waitlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geckovision-tech/openapi/geckovision-tech-waitlist-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: geckovision.tech
  spf: true
hosts:
- cert_expires: Feb  6 14:32:31 2027 GMT
  host: geckovision.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gecko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gecko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gecko
provider_slug: geckovision-tech
slug: geckovision-tech-domain-security
source_filename: geckovision-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geckovision.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 14:32:31 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: geckovision.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/geckovision-tech/security/geckovision-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Data
- Agents
- Platform
- MCP
---
