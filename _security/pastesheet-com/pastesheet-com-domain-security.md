---
api_specs:
- filename: pastesheet-com-openapi-generated.yml
  format: yaml
  label: pastesheet-com API
  slug: pastesheet-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pastesheet-com/openapi/_ae-authored/pastesheet-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pastesheet.com
  spf: true
hosts:
- cert_expires: Jan 27 18:16:18 2027 GMT
  host: pastesheet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pastesheet Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pastesheet-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: pastesheet-com
provider_slug: pastesheet-com
slug: pastesheet-com-domain-security
source_filename: pastesheet-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pastesheet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 18:16:18 2027 GMT\n  hsts: false\ndomains:\n- domain: pastesheet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pastesheet-com/security/pastesheet-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API
- GoogleSheets
- NoCode
- AI
---
