---
api_specs:
- filename: accordo-dev-openapi-generated.yml
  format: yaml
  label: Accordo API
  slug: accordo-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/accordo-dev/openapi/_ae-authored/accordo-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: accordo.dev
  spf: false
hosts:
- cert_expires: Jan  7 06:23:09 2027 GMT
  host: accordo.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Accordo Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accordo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Accordo
provider_slug: accordo-dev
slug: accordo-dev-domain-security
source_filename: accordo-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: accordo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 06:23:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: accordo.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/accordo-dev/security/accordo-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- AI Agents
- Revenue Operations
- Open Source
---
