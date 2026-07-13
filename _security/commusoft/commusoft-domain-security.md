---
api_specs:
- filename: commusoft-api-openapi.yml
  format: yaml
  label: Commusoft API
  slug: commusoft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commusoft/refs/heads/main/openapi/commusoft-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: commusoft.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiary.io
  spf: true
hosts:
- cert_expires: Aug  7 14:04:37 2026 GMT
  host: www.commusoft.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: commusoft.docs.apiary.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.commusoft.com
  https: false
kind: domain-security
layout: security
method: probed
name: Commusoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commusoft, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Commusoft
provider_slug: commusoft
slug: commusoft-domain-security
source_filename: commusoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.commusoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 14:04:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: commusoft.docs.apiary.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\n- host: api.commusoft.com\n  https: false\ndomains:\n- domain: commusoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: apiary.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commusoft/refs/heads/main/security/commusoft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Field Service Management
- Job Management
- HVAC
- Plumbing
- Trades
- Scheduling
- Invoicing
- Engineers
- Customers
- Service History
---
