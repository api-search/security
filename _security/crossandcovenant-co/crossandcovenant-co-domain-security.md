---
api_specs:
- filename: crossandcovenant-co-openapi.yaml
  format: yaml
  label: Cross + Covenant Agent API
  slug: agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crossandcovenant-co/openapi/_original/crossandcovenant-co-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crossandcovenant.co
  spf: true
hosts:
- cert_expires: Nov 29 18:36:40 2026 GMT
  host: crossandcovenant.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crossandcovenant Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for crossandcovenant-co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: crossandcovenant-co
provider_slug: crossandcovenant-co
slug: crossandcovenant-co-domain-security
source_filename: crossandcovenant-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crossandcovenant.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 18:36:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crossandcovenant.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/crossandcovenant-co/security/crossandcovenant-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apparel
- Christian
- E‑commerce
- Faith
- Charity
---
