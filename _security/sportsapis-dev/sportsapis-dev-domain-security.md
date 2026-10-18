---
api_specs:
- filename: sportsapis-dev-openapi-generated.yml
  format: yaml
  label: SportsAPIs.dev API
  slug: sportsapis-dev-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsapis-dev/refs/heads/main/openapi/_ae-authored/sportsapis-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sportsapis.dev
  spf: true
hosts:
- cert_expires: Dec 12 22:05:37 2026 GMT
  host: sportsapis.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sportsapis Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SportsAPIs.dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SportsAPIs.dev
provider_slug: sportsapis-dev
slug: sportsapis-dev-domain-security
source_filename: sportsapis-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sportsapis.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 22:05:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sportsapis.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportsapis-dev/refs/heads/main/security/sportsapis-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sports
- Odds
- Data
- Gambling
---
