---
api_specs:
- filename: karakeep-openapi-generated.yml
  format: yaml
  label: Karakeep API
  slug: karakeep-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/karakeep/openapi/_ae-authored/karakeep-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: karakeep.com
  spf: true
hosts:
- cert_expires: Jan 23 09:19:05 2027 GMT
  host: karakeep.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Karakeep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Karakeep, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Karakeep
provider_slug: karakeep
slug: karakeep-domain-security
source_filename: karakeep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: karakeep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 09:19:05 2027 GMT\n  hsts: false\ndomains:\n- domain: karakeep.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/karakeep/security/karakeep-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Bookmarking
- AI
- Collaboration
- OpenSource
---
