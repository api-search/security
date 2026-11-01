---
api_specs:
- filename: maxxwell-dev-openapi-generated.yml
  format: yaml
  label: Rindler API
  slug: maxxwell-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxxwell-dev/openapi/_ae-authored/maxxwell-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: maxxwell.dev
  spf: true
hosts:
- cert_expires: Jan 15 21:02:30 2027 GMT
  host: maxxwell.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Maxxwell Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rindler, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rindler
provider_slug: maxxwell-dev
slug: maxxwell-dev-domain-security
source_filename: maxxwell-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maxxwell.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 21:02:30 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: maxxwell.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/maxxwell-dev/security/maxxwell-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- DeveloperTools
- OpenSource
- Automation
---
