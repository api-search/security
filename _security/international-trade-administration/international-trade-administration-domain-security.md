---
api_specs:
- filename: international-trade-administration-consolidated-screening-list-api-openapi.yml
  format: yaml
  label: International Trade Administration Consolidated Screening List API
  slug: international-trade-administration-consolidated-screening-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-consolidated-screening-list-api-openapi.yml
- filename: international-trade-administration-country-commercial-guides-api-openapi.yml
  format: yaml
  label: International Trade Administration Country Commercial Guides API
  slug: international-trade-administration-country-commercial-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-country-commercial-guides-api-openapi.yml
- filename: international-trade-administration-customs-tariff-api-openapi.yml
  format: yaml
  label: International Trade Administration Customs Tariff API
  slug: international-trade-administration-customs-tariff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-customs-tariff-api-openapi.yml
- filename: international-trade-administration-de-minimis-api-openapi.yml
  format: yaml
  label: International Trade Administration De Minimis API
  slug: international-trade-administration-de-minimis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-de-minimis-api-openapi.yml
- filename: international-trade-administration-market-intelligence-api-openapi.yml
  format: yaml
  label: International Trade Administration Market Intelligence API
  slug: international-trade-administration-market-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-market-intelligence-api-openapi.yml
- filename: international-trade-administration-trade-events-api-openapi.yml
  format: yaml
  label: International Trade Administration Trade Events API
  slug: international-trade-administration-trade-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-trade-events-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: trade.gov
  spf: true
hosts:
- cert_expires: Jul 28 10:56:42 2026 GMT
  host: developer.trade.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 28 10:56:42 2026 GMT
  host: www.trade.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: data.trade.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: International Trade Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for International Trade Administration, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: International Trade Administration
provider_slug: international-trade-administration
slug: international-trade-administration-domain-security
source_filename: international-trade-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.trade.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 10:56:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.trade.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 10:56:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.trade.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trade.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/security/international-trade-administration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Compliance
- Customs
- Export
- Federal-Government
- International Business
- Screening List
- Tariffs
- Trade
- Trade Data
- Trade Events
---
