---
api_specs:
- filename: freehire-me-api-openapi.yml
  format: yaml
  label: freehire public API API
  slug: freehire-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freehire-me/openapi/_original/freehire-me-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freehire.me
  spf: true
hosts:
- cert_expires: Jan 12 02:52:56 2027 GMT
  host: freehire.me
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Freehire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freehire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Freehire
provider_slug: freehire-me
slug: freehire-me-domain-security
source_filename: freehire-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freehire.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 02:52:56 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: freehire.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/freehire-me/security/freehire-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Job Search
- Open Source
- Tech Jobs
- CLI
---
