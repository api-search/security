---
api_specs:
- filename: selectel-openapi-generated.yml
  format: yaml
  label: Selectel API
  slug: selectel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/selectel/openapi/_ae-authored/selectel-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: selectel.ru
  spf: true
hosts:
- cert_expires: Dec 16 20:34:04 2026 GMT
  host: selectel.ru
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Selectel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Selectel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Selectel
provider_slug: selectel
slug: selectel-domain-security
source_filename: selectel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: selectel.ru\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 16 20:34:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: selectel.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/selectel/security/selectel-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Cloud
- Infrastructure
- VPS
- Storage
- Kubernetes
---
