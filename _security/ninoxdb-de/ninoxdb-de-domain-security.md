---
api_specs:
- filename: ninoxdb-de-openapi-generated.yml
  format: yaml
  label: Ninox API
  slug: ninoxdb-de-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ninoxdb-de/openapi/_ae-authored/ninoxdb-de-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ninoxdb.de
  spf: true
hosts:
- cert_expires: Dec 30 01:38:03 2026 GMT
  host: ninoxdb.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ninoxdb De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ninox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ninox
provider_slug: ninoxdb-de
slug: ninoxdb-de-domain-security
source_filename: ninoxdb-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ninoxdb.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 01:38:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ninoxdb.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ninoxdb-de/security/ninoxdb-de-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Low-code
- Platform
- Business Apps
- Database
---
