---
api_specs:
- filename: flueid-pro-openapi.yml
  format: yaml
  label: Flueid Pro API
  slug: flueid-pro
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-pro-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flueid.com
  spf: true
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: www.flueid.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: pro.flueid.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api.pro.flueid.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Flueid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flueid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flueid
provider_slug: flueid
slug: flueid-domain-security
source_filename: flueid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flueid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: false\n- host: pro.flueid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.pro.flueid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: flueid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/security/flueid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Title Insurance
- Mortgage
- Property Data
- Verification of Title
- Financial Services
- Lending
- PropTech
- Settlement Services
---
