---
api_specs:
- filename: patchmon-scoped-api-hosts-api-openapi.yml
  format: yaml
  label: PatchMon Scoped API - Hosts API
  slug: patchmon-scoped-api-hosts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/patchmon/openapi/patchmon-scoped-api-hosts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: patchmon.net
  spf: true
hosts:
- cert_expires: Nov  3 15:40:04 2026 GMT
  host: patchmon.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Patchmon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PatchMon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PatchMon
provider_slug: patchmon
slug: patchmon-domain-security
source_filename: patchmon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: patchmon.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 15:40:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: patchmon.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/patchmon/security/patchmon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Patch Management
- Linux
- FreeBSD
- Windows
- Open Source
---
