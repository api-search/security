---
api_specs:
- filename: vts-openapi.yml
  format: yaml
  label: VTS Lease API
  slug: vts-lease-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vts/refs/heads/main/openapi/vts-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vts.com
  spf: true
hosts:
- cert_expires: Sep  5 16:46:23 2026 GMT
  host: vts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: api.vts.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: sandbox.vts.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VTS, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VTS
provider_slug: vts
slug: vts-domain-security
source_filename: vts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 16:46:23 2026 GMT\n  hsts: null\n- host: api.vts.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\n- host: sandbox.vts.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: vts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vts/refs/heads/main/security/vts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commercial Real Estate
- PropTech
- Real Estate
- Leasing
- Asset Management
- Property Management
- Tenant Experience
---
