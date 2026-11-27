---
api_specs:
- filename: 2oapi-xyz-openapi-generated.yml
  format: yaml
  label: 2O API
  slug: 2oapi-xyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/2oapi-xyz/openapi/_ae-authored/2oapi-xyz-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 2oapi.xyz
  spf: true
hosts:
- cert_expires: Jan 28 03:44:39 2027 GMT
  host: 2oapi.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 2O Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 2O, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 2O
provider_slug: 2oapi-xyz
slug: 2oapi-xyz-domain-security
source_filename: 2oapi-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 2oapi.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 03:44:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 2oapi.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/2oapi-xyz/security/2oapi-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Verification
- Human-in-the-Loop
- Trust
- Agents
---
