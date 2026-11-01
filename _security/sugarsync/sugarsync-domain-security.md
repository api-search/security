---
api_specs:
- filename: sugarsync-openapi-generated.yml
  format: yaml
  label: SugarSync API
  slug: sugarsync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sugarsync/openapi/_ae-authored/sugarsync-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sugarsync.com
  spf: true
hosts:
- cert_expires: Jan  4 04:49:52 2027 GMT
  host: www1.sugarsync.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sugarsync Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SugarSync, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SugarSync
provider_slug: sugarsync
slug: sugarsync-domain-security
source_filename: sugarsync-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www1.sugarsync.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 04:49:52 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: sugarsync.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/sugarsync/security/sugarsync-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Storage
- File Sync
- Backup
- Collaboration
- Business
---
