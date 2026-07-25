---
api_specs:
- filename: department-of-the-treasury-auctions-api-openapi.yml
  format: yaml
  label: Department of the Treasury Auctions API
  slug: department-of-the-treasury-auctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-auctions-api-openapi.yml
- filename: department-of-the-treasury-debt-api-openapi.yml
  format: yaml
  label: Department of the Treasury Debt API
  slug: department-of-the-treasury-debt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-debt-api-openapi.yml
- filename: department-of-the-treasury-exchange-rates-api-openapi.yml
  format: yaml
  label: Department of the Treasury Exchange Rates API
  slug: department-of-the-treasury-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-exchange-rates-api-openapi.yml
- filename: department-of-the-treasury-interest-rates-api-openapi.yml
  format: yaml
  label: Department of the Treasury Interest Rates API
  slug: department-of-the-treasury-interest-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-interest-rates-api-openapi.yml
- filename: department-of-the-treasury-sanctions-lists-api-openapi.yml
  format: yaml
  label: Department of the Treasury Sanctions Lists API
  slug: department-of-the-treasury-sanctions-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-sanctions-lists-api-openapi.yml
- filename: department-of-the-treasury-search-api-openapi.yml
  format: yaml
  label: Department of the Treasury Search API
  slug: department-of-the-treasury-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-search-api-openapi.yml
- filename: department-of-the-treasury-spending-api-openapi.yml
  format: yaml
  label: Department of the Treasury Spending API
  slug: department-of-the-treasury-spending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-spending-api-openapi.yml
- filename: department-of-the-treasury-treasury-operations-api-openapi.yml
  format: yaml
  label: Department of the Treasury Treasury Operations API
  slug: department-of-the-treasury-treasury-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-treasury-operations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: treasury.gov
  spf: true
hosts:
- cert_expires: Sep 23 21:25:47 2026 GMT
  host: home.treasury.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: fiscaldata.treasury.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: api.fiscaldata.treasury.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Department Of The Treasury Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Department of the Treasury, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Department of the Treasury
provider_slug: department-of-the-treasury
slug: department-of-the-treasury-domain-security
source_filename: department-of-the-treasury-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: home.treasury.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:25:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fiscaldata.treasury.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fiscaldata.treasury.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: treasury.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/security/department-of-the-treasury-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Finance
- Debt
- Sanctions
---
