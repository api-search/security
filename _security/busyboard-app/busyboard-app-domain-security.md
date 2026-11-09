---
api_specs:
- filename: busyboard-app-api-openapi.yml
  format: yaml
  label: BusyBoard API API
  slug: busyboard-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/busyboard-app/openapi/_original/busyboard-app-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: busyboard.app
  spf: true
hosts:
- cert_expires: Dec  9 19:51:31 2026 GMT
  host: busyboard.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Busyboard App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BusyBoard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BusyBoard
provider_slug: busyboard-app
slug: busyboard-app-domain-security
source_filename: busyboard-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: busyboard.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 19:51:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: busyboard.app\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/busyboard-app/security/busyboard-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Scheduling
- Calendar
- Privacy
- Free
- Software-as-a-Service
---
