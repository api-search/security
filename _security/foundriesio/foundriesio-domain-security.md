---
api_specs:
- filename: foundriesio-openapi-generated.yml
  format: yaml
  label: Foundries.io API
  slug: foundriesio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundriesio/openapi/_ae-authored/foundriesio-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: foundries.io
  spf: true
hosts:
- cert_expires: Jan  4 18:52:07 2027 GMT
  host: www.foundries.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foundriesio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foundries.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Foundries.io
provider_slug: foundriesio
slug: foundriesio-domain-security
source_filename: foundriesio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foundries.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 18:52:07 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: foundries.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/foundriesio/security/foundriesio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- IoT
- Embedded-Linux
- Edge-Computing
- Device-Management
- Secure-Updates
---
