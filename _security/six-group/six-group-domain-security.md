---
api_specs:
- filename: downloads
  format: yaml
  label: SIX bLink API
  slug: blink-api
  spec_type: Postman
  url: https://docs.blink.six-group.com/docs/downloads
- filename: six-group-card-management-api-openapi.yml
  format: yaml
  label: SIX debiX API
  slug: debix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/six-group/refs/heads/main/openapi/six-group-card-management-api-openapi.yml
- filename: six-group-3ds-authentication-api-openapi.yml
  format: yaml
  label: SIX debiX Auth Provider API
  slug: debix-auth-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/six-group/refs/heads/main/openapi/six-group-3ds-authentication-api-openapi.yml
- filename: six-group-bankmaster-api-openapi.yml
  format: yaml
  label: Swiss Bank Master API
  slug: swiss-bank-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/six-group/refs/heads/main/openapi/six-group-bankmaster-api-openapi.yml
- filename: six-group-status-api-openapi.yml
  format: yaml
  label: SIC Service Status API
  slug: sic-service-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/six-group/refs/heads/main/openapi/six-group-status-api-openapi.yml
- filename: six-group-calendar-api-openapi.yml
  format: yaml
  label: SIC Clearing Day Calendar API
  slug: sic-clearing-day-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/six-group/refs/heads/main/openapi/six-group-calendar-api-openapi.yml
- filename: six-group-detailedsettlementinformation-api-openapi.yml
  format: yaml
  label: Settlement Info Reporting API
  slug: settlement-info-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/six-group/refs/heads/main/openapi/six-group-detailedsettlementinformation-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "swisssign.com"
  - 0 issue "amazonaws.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazontrust.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: six-group.com
  spf: true
hosts:
- cert_expires: Nov 27 07:51:16 2026 GMT
  host: www.six-group.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 08:12:23 2026 GMT
  host: developer.six-group.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: docs.blink.six-group.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Six Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SIX, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SIX
provider_slug: six-group
slug: six-group-domain-security
source_filename: six-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.six-group.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 07:51:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.six-group.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 08:12:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.blink.six-group.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: six-group.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"swisssign.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/six-group/refs/heads/main/security/six-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Market Data
- Stocks
- Reference Data
- Corporate Actions
- Real-Time
- Exchange
- Open Banking
- Payments
- Switzerland
---
