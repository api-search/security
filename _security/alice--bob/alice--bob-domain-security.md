---
api_specs:
- filename: alice--bob-health-api-openapi.yml
  format: yaml
  label: Alice Bob Health API
  slug: alice--bob-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice--bob/refs/heads/main/openapi/alice--bob-health-api-openapi.yml
- filename: alice--bob-jobs-api-openapi.yml
  format: yaml
  label: Alice Bob Jobs API
  slug: alice--bob-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice--bob/refs/heads/main/openapi/alice--bob-jobs-api-openapi.yml
- filename: alice--bob-targets-api-openapi.yml
  format: yaml
  label: Alice Bob Targets API
  slug: alice--bob-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice--bob/refs/heads/main/openapi/alice--bob-targets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alice-bob.com
  spf: true
hosts:
- cert_expires: Oct 16 09:04:09 2026 GMT
  host: alice-bob.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 01:12:50 2026 GMT
  host: felis.alice-bob.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 15:24:24 2026 GMT
  host: api-gcp.alice-bob.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alice  Bob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alice Bob, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alice Bob
provider_slug: alice--bob
slug: alice--bob-domain-security
source_filename: alice--bob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alice-bob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 09:04:09 2026 GMT\n  hsts: false\n- host: felis.alice-bob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 01:12:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api-gcp.alice-bob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 15:24:24 2026 GMT\n  hsts: null\ndomains:\n- domain: alice-bob.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alice--bob/refs/heads/main/security/alice--bob-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Quantum Computing
- Quantum
- Cloud Computing
- Emulation
- Developer Tools
- Compute
- Hardware
- Research
- Qiskit
- QIR
---
