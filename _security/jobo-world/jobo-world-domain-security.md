---
api_specs:
- filename: jobo-world-openapi-generated.yml
  format: yaml
  label: jobo-world API
  slug: jobo-world-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobo-world/openapi/_ae-authored/jobo-world-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jobo.world
  spf: true
hosts:
- cert_expires: Dec  9 17:24:00 2026 GMT
  host: jobo.world
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jobo World Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for jobo-world, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: jobo-world
provider_slug: jobo-world
slug: jobo-world-domain-security
source_filename: jobo-world-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jobo.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 17:24:00 2026 GMT\n  hsts: null\ndomains:\n- domain: jobo.world\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jobo-world/security/jobo-world-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Job Data
- API
- Recruitment
- Platform
- Data Infrastructure
---
