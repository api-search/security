---
api_specs:
- filename: meku-farm-openapi-generated.yml
  format: yaml
  label: MEKU API
  slug: meku-farm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meku-farm/openapi/_ae-authored/meku-farm-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meku.farm
  spf: true
hosts:
- cert_expires: Jan  1 10:37:02 2027 GMT
  host: meku.farm
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MEKU Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MEKU, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MEKU
provider_slug: meku-farm
slug: meku-farm-domain-security
source_filename: meku-farm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meku.farm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 10:37:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: meku.farm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/meku-farm/security/meku-farm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Human-AI
- Platform
- FreeDemo
- NoPayments
- Open Source
---
