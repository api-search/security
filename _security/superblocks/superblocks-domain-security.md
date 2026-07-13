---
api_specs:
- filename: openapi.json
  format: json
  label: Superblocks Management API
  slug: superblocks-api
  spec_type: OpenAPI
  url: https://docs.superblocks.com/api-reference/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: superblocks.com
  spf: true
hosts:
- cert_expires: Sep 10 05:47:57 2026 GMT
  host: www.superblocks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 06:02:27 2026 GMT
  host: docs.superblocks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: api.superblocks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superblocks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superblocks, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Superblocks
provider_slug: superblocks
slug: superblocks-domain-security
source_filename: superblocks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.superblocks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 05:47:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.superblocks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 06:02:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.superblocks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: superblocks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superblocks/refs/heads/main/security/superblocks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- internal tools
- low-code
- no-code
- applications
- workflows
- scheduled jobs
- integrations
- enterprise
- AI
- databases
- REST API
- developer tools
---
