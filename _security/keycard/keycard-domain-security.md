---
api_specs:
- filename: keycard-keycard-api-api-openapi.yml
  format: yaml
  label: Keycard API
  slug: keycard-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keycard/openapi/keycard-keycard-api-api-openapi.yml
- filename: keycard-openapi-generated.yml
  format: yaml
  label: Keycard API
  slug: keycard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keycard/openapi/_ae-authored/keycard-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: keycard.sh
  spf: true
hosts:
- cert_expires: Nov 28 19:43:28 2026 GMT
  host: keycard.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Keycard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keycard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Keycard
provider_slug: keycard
slug: keycard-domain-security
source_filename: keycard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keycard.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 19:43:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: keycard.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/keycard/security/keycard-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Authentication
- Authorization
- Identity
- Agent Security
- Policy as Code
- Runtime Access
---
