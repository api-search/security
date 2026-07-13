---
api_specs:
- filename: schema.json
  format: json
  label: Baserow REST API
  slug: baserow-rest-api
  spec_type: OpenAPI
  url: https://api.baserow.io/api/schema.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: baserow.io
  spf: true
hosts:
- cert_expires: Sep 11 07:41:56 2026 GMT
  host: baserow.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 15:55:46 2026 GMT
  host: api.baserow.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Baserow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baserow, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Baserow
provider_slug: baserow
slug: baserow-domain-security
source_filename: baserow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: baserow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 07:41:56 2026 GMT\n  hsts: false\n- host: api.baserow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:55:46 2026 GMT\n  hsts: null\ndomains:\n- domain: baserow.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baserow/refs/heads/main/security/baserow-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- No-Code
- Database
- Open Source
- REST API
- Self-Hosted
- Tables
- Rows
- Automation
---
