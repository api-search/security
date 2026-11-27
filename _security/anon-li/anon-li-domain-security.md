---
api_specs:
- filename: anon-li-openapi-generated.yml
  format: yaml
  label: anon.li API
  slug: anon-li-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anon-li/openapi/_ae-authored/anon-li-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anon.li
  spf: true
hosts:
- cert_expires: Dec  6 23:29:48 2026 GMT
  host: anon.li
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: anon.li Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for anon.li, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: anon.li
provider_slug: anon-li
slug: anon-li-domain-security
source_filename: anon-li-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anon.li\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:29:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: anon.li\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/anon-li/security/anon-li-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Privacy
- Email
- Encryption
- File Sharing
- Forms
---
