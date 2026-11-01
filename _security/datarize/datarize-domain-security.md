---
api_specs:
- filename: datarize-openapi-generated.yml
  format: yaml
  label: Datarize API
  slug: datarize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datarize/openapi/_ae-authored/datarize-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datarize.ai
  spf: true
hosts:
- cert_expires: Dec  1 03:51:27 2026 GMT
  host: www.datarize.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datarize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datarize, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Datarize
provider_slug: datarize
slug: datarize-domain-security
source_filename: datarize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datarize.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 03:51:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datarize.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/datarize/security/datarize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Integration
- Analytics
- API Platform
- Enterprise
---
