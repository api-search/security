---
api_specs:
- filename: instadash-io-openapi-generated.yml
  format: yaml
  label: Instadash API
  slug: instadash-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instadash-io/openapi/_ae-authored/instadash-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: instadash.io
  spf: true
hosts:
- cert_expires: Feb  4 05:57:52 2027 GMT
  host: instadash.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Instadash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instadash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Instadash
provider_slug: instadash-io
slug: instadash-io-domain-security
source_filename: instadash-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instadash.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 05:57:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: instadash.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/instadash-io/security/instadash-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Data
- Ingestion
- Mesh
- Platform
- Company
---
