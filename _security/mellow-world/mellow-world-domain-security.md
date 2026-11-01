---
api_specs:
- filename: mellow-world-openapi-generated.yml
  format: yaml
  label: mellow-world API
  slug: mellow-world-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mellow-world/openapi/_ae-authored/mellow-world-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mellow.world
  spf: true
hosts:
- cert_expires: Dec 22 11:53:56 2026 GMT
  host: mellow.world
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mellow World Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mellow-world, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mellow-world
provider_slug: mellow-world
slug: mellow-world-domain-security
source_filename: mellow-world-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mellow.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 11:53:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mellow.world\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mellow-world/security/mellow-world-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social Media
- Marketing
- Scheduling
- Content Creation
- SaaS
---
