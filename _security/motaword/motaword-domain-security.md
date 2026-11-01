---
api_specs:
- filename: motaword-api-openapi.yml
  format: yaml
  label: MotaWord API API
  slug: motaword-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/motaword/openapi/_original/motaword-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: motaword.com
  spf: true
hosts:
- cert_expires: Jan  5 13:13:14 2027 GMT
  host: motaword.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Motaword Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MotaWord, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MotaWord
provider_slug: motaword
slug: motaword-domain-security
source_filename: motaword-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motaword.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 13:13:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: motaword.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/motaword/security/motaword-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Translation
- Localization
- AI
- SaaS
- Enterprise
---
