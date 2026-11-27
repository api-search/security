---
api_specs:
- filename: garmolabs-com-openapi-generated.yml
  format: yaml
  label: Garmo Labs API
  slug: garmolabs-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/garmolabs-com/openapi/_ae-authored/garmolabs-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: garmolabs.com
  spf: true
hosts:
- cert_expires: Dec 10 20:57:01 2026 GMT
  host: garmolabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Garmo Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Garmo Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Garmo Labs
provider_slug: garmolabs-com
slug: garmolabs-com-domain-security
source_filename: garmolabs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: garmolabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 20:57:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: garmolabs.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/garmolabs-com/security/garmolabs-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Semiconductor IP
- Chip Architecture
- Software Platform
- AI Compute
- Developer Tools
- Research Benchmarks
---
