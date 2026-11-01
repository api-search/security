---
api_specs:
- filename: avian-openapi-generated.yml
  format: yaml
  label: Avian.io API
  slug: avian-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avian/openapi/_ae-authored/avian-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: avian.io
  spf: true
hosts:
- cert_expires: Dec 30 11:50:44 2026 GMT
  host: avian.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avian.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Avian.io
provider_slug: avian
slug: avian-domain-security
source_filename: avian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avian.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 11:50:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: avian.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/avian/security/avian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Inference
- Compute
- OpenAI Compatibility
- GPU Compute
- Enterprise Security
---
