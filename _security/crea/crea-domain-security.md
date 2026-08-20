---
api_specs:
- filename: crea-realtor-ca-ddf-web-api-openapi.json
  format: json
  label: REALTOR.ca DDF Web API
  slug: realtor-ca-ddf-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crea/refs/heads/main/openapi/crea-realtor-ca-ddf-web-api-openapi.json
- filename: crea-realtor-ca-ddf-web-api-openapi.json
  format: json
  label: REALTOR.ca DDF Lead API
  slug: realtor-ca-ddf-lead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crea/refs/heads/main/openapi/crea-realtor-ca-ddf-web-api-openapi.json
- filename: crea-realtor-ca-board-api-openapi.json
  format: json
  label: REALTOR.ca Board API
  slug: realtor-ca-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crea/refs/heads/main/openapi/crea-realtor-ca-board-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crea.ca
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: realtor.ca
  spf: true
hosts:
- cert_expires: Sep 25 07:36:09 2026 GMT
  host: www.crea.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:31:29 2026 GMT
  host: www.realtor.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:31:29 2026 GMT
  host: ddfapi-docs.realtor.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CREA (REALTOR.ca), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CREA (REALTOR.ca)
provider_slug: crea
slug: crea-domain-security
source_filename: crea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crea.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 07:36:09 2026 GMT\n  hsts: false\n- host: www.realtor.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:31:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ddfapi-docs.realtor.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:31:29 2026 GMT\n  hsts: null\ndomains:\n- domain: crea.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: realtor.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crea/refs/heads/main/security/crea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- Canada
- Property Listings
- MLS
- IDX
- RESO
- OData
- Industry Body
- PropTech
- Data Syndication
---
