---
api_specs:
- filename: fidro-io-openapi-generated.yml
  format: yaml
  label: fidro-io API
  slug: fidro-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fidro-io/openapi/_ae-authored/fidro-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fidro.io
  spf: false
hosts:
- cert_expires: Jan 11 10:33:54 2027 GMT
  host: fidro.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fidro Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fidro-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: fidro-io
provider_slug: fidro-io
slug: fidro-io-domain-security
source_filename: fidro-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fidro.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 10:33:54 2027 GMT\n  hsts: false\ndomains:\n- domain: fidro.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fidro-io/security/fidro-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- FraudDetection
- API
- RiskAnalysis
- Payments
---
