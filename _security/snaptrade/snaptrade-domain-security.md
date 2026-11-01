---
api_specs:
- filename: snaptrade-account-information-api-openapi.yml
  format: yaml
  label: SnapTrade Account Information API
  slug: snaptrade-account-information-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaptrade/openapi/snaptrade-account-information-api-openapi.yml
- filename: snaptrade-api-status-api-openapi.yml
  format: yaml
  label: SnapTrade API Status API
  slug: snaptrade-api-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaptrade/openapi/snaptrade-api-status-api-openapi.yml
- filename: snaptrade-authentication-api-openapi.yml
  format: yaml
  label: SnapTrade Authentication API
  slug: snaptrade-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaptrade/openapi/snaptrade-authentication-api-openapi.yml
- filename: snaptrade-connections-api-openapi.yml
  format: yaml
  label: SnapTrade Connections API
  slug: snaptrade-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaptrade/openapi/snaptrade-connections-api-openapi.yml
- filename: snaptrade-management-api-openapi.yml
  format: yaml
  label: SnapTrade Management API
  slug: snaptrade-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaptrade/openapi/snaptrade-management-api-openapi.yml
- filename: snaptrade-reference-data-api-openapi.yml
  format: yaml
  label: SnapTrade Reference Data API
  slug: snaptrade-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaptrade/openapi/snaptrade-reference-data-api-openapi.yml
- filename: snaptrade-trading-api-openapi.yml
  format: yaml
  label: SnapTrade Trading API
  slug: snaptrade-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaptrade/openapi/snaptrade-trading-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 iodef "mailto:security@snaptrade.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: snaptrade.com
  spf: true
hosts:
- cert_expires: Apr 30 08:30:47 2027 GMT
  host: snaptrade.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Snaptrade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SnapTrade, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SnapTrade
provider_slug: snaptrade
slug: snaptrade-domain-security
source_filename: snaptrade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snaptrade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 30 08:30:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: snaptrade.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 iodef \"mailto:security@snaptrade.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/snaptrade/security/snaptrade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Brokerage
- Trading
---
