---
api_specs:
- filename: aihcc-cloud-openapi-generated.yml
  format: yaml
  label: AIHCC API
  slug: aihcc-cloud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihcc-cloud/openapi/_ae-authored/aihcc-cloud-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aihcc.cloud
  spf: false
hosts:
- cert_expires: Jan 26 07:49:57 2027 GMT
  host: aihcc.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aihcc Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIHCC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AIHCC
provider_slug: aihcc-cloud
slug: aihcc-cloud-domain-security
source_filename: aihcc-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aihcc.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 07:49:57 2027 GMT\n  hsts: false\ndomains:\n- domain: aihcc.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aihcc-cloud/security/aihcc-cloud-domain-security.yml
summary_line: TLSv1.3
tags:
- AI Safety
- Agent Tools
- Hallucination Detection
- Prompt Injection
- Chinese
---
