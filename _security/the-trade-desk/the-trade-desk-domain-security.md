---
api_specs:
- filename: the-trade-desk-advertiser-api-openapi.yml
  format: yaml
  label: The Trade Desk Advertiser API
  slug: the-trade-desk-advertiser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-trade-desk/refs/heads/main/openapi/the-trade-desk-advertiser-api-openapi.yml
- filename: the-trade-desk-deletionoptout-api-openapi.yml
  format: yaml
  label: The Trade Desk DeletionOptOut API
  slug: the-trade-desk-deletionoptout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-trade-desk/refs/heads/main/openapi/the-trade-desk-deletionoptout-api-openapi.yml
- filename: the-trade-desk-offlineconversion-api-openapi.yml
  format: yaml
  label: The Trade Desk OfflineConversion API
  slug: the-trade-desk-offlineconversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-trade-desk/refs/heads/main/openapi/the-trade-desk-offlineconversion-api-openapi.yml
- filename: the-trade-desk-thirdparty-api-openapi.yml
  format: yaml
  label: The Trade Desk ThirdParty API
  slug: the-trade-desk-thirdparty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-trade-desk/refs/heads/main/openapi/the-trade-desk-thirdparty-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thetradedesk.com
  spf: true
hosts:
- cert_expires: Apr  2 07:59:59 2027 GMT
  host: partner.thetradedesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 15:06:16 2026 GMT
  host: www.thetradedesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 07:59:59 2027 GMT
  host: api.thetradedesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Trade Desk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Trade Desk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Trade Desk
provider_slug: the-trade-desk
slug: the-trade-desk-domain-security
source_filename: the-trade-desk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: partner.thetradedesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 07:59:59 2027 GMT\n  hsts: null\n- host: www.thetradedesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 15:06:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.thetradedesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 07:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: thetradedesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-trade-desk/refs/heads/main/security/the-trade-desk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Programmatic Advertising
- DSP
- Demand-Side Platform
- Campaign Management
- Connected TV
- Digital Advertising
- Marketing
- AdTech
---
