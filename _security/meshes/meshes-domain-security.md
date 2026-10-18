---
api_specs:
- filename: meshes-openapi-generated.yml
  format: yaml
  label: Meshes API
  slug: meshes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meshes/refs/heads/main/openapi/_ae-authored/meshes-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: meshes.io
  spf: true
hosts:
- cert_expires: Jan  7 15:20:51 2027 GMT
  host: meshes.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Meshes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meshes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Meshes
provider_slug: meshes
slug: meshes-domain-security
source_filename: meshes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meshes.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 15:20:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: meshes.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meshes/refs/heads/main/security/meshes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- iPaaS
- SaaS
- Integration
- API
---
