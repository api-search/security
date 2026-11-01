---
api_specs:
- filename: gapup-io-openapi-generated.yml
  format: yaml
  label: gapup-io API
  slug: gapup-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gapup-io/openapi/_ae-authored/gapup-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gapup.io
  spf: true
hosts:
- cert_expires: Jan 23 14:25:36 2027 GMT
  host: gapup.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gapup Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for gapup-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: gapup-io
provider_slug: gapup-io
slug: gapup-io-domain-security
source_filename: gapup-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gapup.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 14:25:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gapup.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gapup-io/security/gapup-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Finance
- Operations
- Compliance
- Enterprise
---
