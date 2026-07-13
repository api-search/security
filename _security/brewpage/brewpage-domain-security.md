---
api_specs:
- filename: brewpage-openapi.yml
  format: yaml
  label: BrewPage API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brewpage/refs/heads/main/openapi/brewpage-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brewpage.app
  spf: true
hosts:
- cert_expires: Oct  8 18:17:13 2026 GMT
  host: brewpage.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brewpage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrewPage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BrewPage
provider_slug: brewpage
slug: brewpage-domain-security
source_filename: brewpage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brewpage.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:17:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: brewpage.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brewpage/refs/heads/main/security/brewpage-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Hosting
- Markdown
- HTML
- AI Artifacts
- File Hosting
- Developer Tools
---
