---
api_specs:
- filename: mattercatalog-openapi-generated.yml
  format: yaml
  label: MatterCatalog API
  slug: mattercatalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mattercatalog/openapi/_ae-authored/mattercatalog-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mattercatalog.com
  spf: true
hosts:
- cert_expires: Jan 21 12:36:28 2027 GMT
  host: mattercatalog.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MatterCatalog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MatterCatalog, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MatterCatalog
provider_slug: mattercatalog
slug: mattercatalog-domain-security
source_filename: mattercatalog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mattercatalog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 12:36:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: mattercatalog.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mattercatalog/security/mattercatalog-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Matter
- Smart Home
- IoT
- Certification
- Directory
---
