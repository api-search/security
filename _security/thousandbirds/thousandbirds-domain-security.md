---
api_specs:
- filename: thousandbirds-openapi-generated.yml
  format: yaml
  label: ThousandBirds API
  slug: thousandbirds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thousandbirds/openapi/_ae-authored/thousandbirds-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thousandbirds.ai
  spf: false
hosts:
- cert_expires: Dec  7 23:40:30 2026 GMT
  host: thousandbirds.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thousandbirds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThousandBirds, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ThousandBirds
provider_slug: thousandbirds
slug: thousandbirds-domain-security
source_filename: thousandbirds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thousandbirds.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:40:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thousandbirds.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/thousandbirds/security/thousandbirds-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Agents
- Debugging
- TypeScript
- Open Source
---
