---
api_specs:
- filename: lighthorse-io-cash-api-openapi.yml
  format: yaml
  label: Light Horse Cash API
  slug: lighthorse-io-cash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lighthorse-io/openapi/lighthorse-io-cash-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lighthorse.io
  spf: true
hosts:
- cert_expires: Jan  3 03:26:37 2027 GMT
  host: lighthorse.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Light Horse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Light Horse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Light Horse
provider_slug: lighthorse-io
slug: lighthorse-io-domain-security
source_filename: lighthorse-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lighthorse.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 03:26:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lighthorse.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lighthorse-io/security/lighthorse-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Brokerage
- Finance
- Trading
---
