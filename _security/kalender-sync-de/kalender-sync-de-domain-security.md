---
api_specs:
- filename: kalender-sync-de-v1-openapi.json
  format: json
  label: Kalender Sync API V1 API
  slug: kalender-sync-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kalender-sync-de/openapi/_original/kalender-sync-de-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kalender-sync.de
  spf: true
hosts:
- cert_expires: Jan  8 12:35:24 2027 GMT
  host: kalender-sync.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kalender Sync Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kalender Sync, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kalender Sync
provider_slug: kalender-sync-de
slug: kalender-sync-de-domain-security
source_filename: kalender-sync-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kalender-sync.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 12:35:24 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kalender-sync.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kalender-sync-de/security/kalender-sync-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
