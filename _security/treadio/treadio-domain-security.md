---
api_specs:
- filename: treadio-horizon-openapi.json
  format: json
  label: Tread Horizon API V1
  slug: tread-horizon-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treadio/refs/heads/main/openapi/treadio-horizon-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tread.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tread-horizon.com
  spf: false
hosts:
- cert_expires: Aug 31 16:28:35 2026 GMT
  host: tread.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: api.tread-horizon.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Treadio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tread.io, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: tread.io
provider_slug: treadio
slug: treadio-domain-security
source_filename: treadio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tread.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:28:35 2026 GMT\n  hsts: false\n- host: api.tread-horizon.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tread.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tread-horizon.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treadio/refs/heads/main/security/treadio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Construction
- Logistics
- Transportation Management
- Dispatch
- Fleet Management
- Bulk Materials
- Trucking
- Webhooks
- API
---
