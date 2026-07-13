---
api_specs:
- filename: column-asyncapi.yml
  format: yaml
  label: Column Webhooks
  slug: column-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: column.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: column.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.column.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: docs.column.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Column Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Column, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Column
provider_slug: column
slug: column-domain-security
source_filename: column-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: column.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: false\n- host: api.column.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\n- host: docs.column.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: column.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/security/column-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fintech
- Banking
- BaaS
- ACH
- Wires
---
