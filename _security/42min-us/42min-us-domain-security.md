---
api_specs:
- filename: 42min-us-api-openapi.yml
  format: yaml
  label: 42min API API
  slug: 42min-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/42min-us/openapi/_original/42min-us-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 42min.us
  spf: true
hosts:
- cert_expires: Jan  6 17:50:04 2027 GMT
  host: 42min.us
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 42Min Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 42min, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 42min
provider_slug: 42min-us
slug: 42min-us-domain-security
source_filename: 42min-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 42min.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 17:50:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 42min.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/42min-us/security/42min-us-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Scheduling
- Free
- Webhook
- Automation
---
