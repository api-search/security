---
api_specs:
- filename: bedrocktap-com-openapi.yml
  format: yaml
  label: BedrockTap API
  slug: bedrocktap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bedrocktap-com/openapi/bedrocktap-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bedrocktap.com
  spf: false
hosts:
- cert_expires: Jan 12 19:29:19 2027 GMT
  host: bedrocktap.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BedrockTap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BedrockTap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: BedrockTap
provider_slug: bedrocktap-com
slug: bedrocktap-com-domain-security
source_filename: bedrocktap-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bedrocktap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 19:29:19 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bedrocktap.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bedrocktap-com/security/bedrocktap-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MCP
- Data Aggregation
- Marketing
- Analytics
---
