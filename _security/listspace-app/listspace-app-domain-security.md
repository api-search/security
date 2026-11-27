---
api_specs:
- filename: listspace-app-openapi-generated.yml
  format: yaml
  label: Listspace API
  slug: listspace-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listspace-app/openapi/_ae-authored/listspace-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: listspace.app
  spf: true
hosts:
- cert_expires: Dec 24 17:34:42 2026 GMT
  host: listspace.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Listspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Listspace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Listspace
provider_slug: listspace-app
slug: listspace-app-domain-security
source_filename: listspace-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: listspace.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 17:34:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: listspace.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/listspace-app/security/listspace-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Collaboration
- Memory
- Agents
- Platform
---
