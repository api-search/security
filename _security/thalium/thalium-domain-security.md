---
api_specs:
- filename: thalium-openapi-generated.yml
  format: yaml
  label: SYSGRAFT API
  slug: thalium-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thalium/openapi/_ae-authored/thalium-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thalium.io
  spf: true
hosts:
- cert_expires: Dec 25 11:00:01 2026 GMT
  host: thalium.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thalium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SYSGRAFT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SYSGRAFT
provider_slug: thalium
slug: thalium-domain-security
source_filename: thalium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thalium.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 11:00:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thalium.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/thalium/security/thalium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Privacy
- Memory API
- Orchestration
---
