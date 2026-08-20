---
api_specs:
- filename: nar-m1-gateway-external-openapi.json
  format: json
  label: REALTORS M1 Gateway External API
  slug: nar-m1-gateway-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nar/refs/heads/main/openapi/nar-m1-gateway-external-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nar.realtor
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: m1gateway.realtor
  spf: false
hosts:
- cert_expires: Aug 29 07:05:36 2026 GMT
  host: www.nar.realtor
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: m1gateway.realtor
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Association of REALTORS, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: National Association of REALTORS
provider_slug: nar
slug: nar-domain-security
source_filename: nar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nar.realtor\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 07:05:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: m1gateway.realtor\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nar.realtor\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: m1gateway.realtor\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nar/refs/heads/main/security/nar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- United States
- Industry Body
- MLS
- RESO
- Standards
- Membership
- Property Listings
- IDX
- PropTech
---
