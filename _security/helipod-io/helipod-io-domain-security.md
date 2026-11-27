---
api_specs:
- filename: helipod-io-container-openapi-generated.yml
  format: yaml
  label: Helipod Container API
  slug: container-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helipod-io/openapi/_ae-authored/helipod-io-container-openapi-generated.yml
- filename: helipod-io-core-openapi-generated.yml
  format: yaml
  label: Helipod core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helipod-io/openapi/_ae-authored/helipod-io-core-openapi-generated.yml
- filename: helipod-io-email-openapi-generated.yml
  format: yaml
  label: Helipod Email API
  slug: email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helipod-io/openapi/_ae-authored/helipod-io-email-openapi-generated.yml
- filename: helipod-io-vps-openapi-generated.yml
  format: yaml
  label: Helipod VPS API
  slug: vps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helipod-io/openapi/_ae-authored/helipod-io-vps-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: helipod.io
  spf: true
hosts:
- cert_expires: Jan 15 09:58:48 2027 GMT
  host: helipod.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Helipod Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helipod, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Helipod
provider_slug: helipod-io
slug: helipod-io-domain-security
source_filename: helipod-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: helipod.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 09:58:48 2027 GMT\n  hsts: null\ndomains:\n- domain: helipod.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/helipod-io/security/helipod-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud
- Platform-as-a-Service
- Indonesia
- Hosting
- Developers
---
