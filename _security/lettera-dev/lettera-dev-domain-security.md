---
api_specs:
- filename: lettera-dev-api-openapi.json
  format: json
  label: Lettera Relay API API
  slug: lettera-relay-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lettera-dev/openapi/_original/lettera-dev-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lettera.dev
  spf: false
hosts:
- cert_expires: Jan 23 10:09:03 2027 GMT
  host: lettera.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lettera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lettera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Lettera
provider_slug: lettera-dev
slug: lettera-dev-domain-security
source_filename: lettera-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lettera.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 10:09:03 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lettera.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lettera-dev/security/lettera-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Artificial Intelligence
- Messaging
- Agents
---
