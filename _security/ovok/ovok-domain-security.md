---
api_specs:
- filename: ovok-openapi-generated.yml
  format: yaml
  label: Ovok API
  slug: ovok-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ovok/openapi/_ae-authored/ovok-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ovok.com
  spf: false
hosts:
- cert_expires: Jan  6 12:50:26 2027 GMT
  host: www.ovok.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ovok Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ovok, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Ovok
provider_slug: ovok
slug: ovok-domain-security
source_filename: ovok-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ovok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 12:50:26 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ovok.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ovok/security/ovok-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- FHIR
- Digital Health
- API Platform
---
