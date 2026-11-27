---
api_specs:
- filename: leeway-tech-public-api-openapi.yml
  format: yaml
  label: Leeway Public API
  slug: leeway-tech-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leeway-tech/openapi/leeway-tech-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leeway.tech
  spf: true
hosts:
- cert_expires: Jan  3 22:12:45 2027 GMT
  host: leeway.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Leeway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leeway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Leeway
provider_slug: leeway-tech
slug: leeway-tech-domain-security
source_filename: leeway-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leeway.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 22:12:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: leeway.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/leeway-tech/security/leeway-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Finance
- Stock Analysis
- Market Research
---
