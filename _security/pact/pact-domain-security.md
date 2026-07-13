---
api_specs:
- filename: pact-openapi.yml
  format: yaml
  label: Pact Broker API
  slug: pact-broker
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pact/refs/heads/main/openapi/pact-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pact.io
  spf: false
hosts:
- cert_expires: Sep  2 02:43:56 2026 GMT
  host: pact.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 03:33:41 2026 GMT
  host: docs.pact.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pact, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Pact
provider_slug: pact
slug: pact-domain-security
source_filename: pact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pact.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 02:43:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pact.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:33:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pact.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pact/refs/heads/main/security/pact-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Contract Testing
- Open Source
- Testing
---
