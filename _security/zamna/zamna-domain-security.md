---
api_specs:
- filename: zamna-paxcheck-openapi-original.json
  format: json
  label: Zamna Ready To Fly (PaxCheck) API
  slug: zamna-ready-to-fly-paxcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zamna/refs/heads/main/openapi/zamna-paxcheck-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zamna.com
  spf: true
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: zamna.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: dev.zamna.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: paxcheck-app-dev.staging.zamna.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zamna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zamna, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zamna
provider_slug: zamna
slug: zamna-domain-security
source_filename: zamna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zamna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: false\n- host: dev.zamna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: false\n- host: paxcheck-app-dev.staging.zamna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: zamna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zamna/refs/heads/main/security/zamna-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aviation
- Travel
- Identity Verification
- Digital Identity
- Passenger Processing
- Airlines
- Border Security
- Document Verification
- KYC
---
