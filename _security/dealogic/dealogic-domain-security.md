---
api_specs:
- filename: dealogic-analytics-spac-v2-openapi.json
  format: json
  label: Dealogic Analytics SPAC API
  slug: dealogic-analytics-spac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-analytics-spac-v2-openapi.json
- filename: dealogic-analytics-bank-openapi.json
  format: json
  label: Dealogic Analytics Bank API
  slug: dealogic-analytics-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-analytics-bank-openapi.json
- filename: dealogic-analytics-company-openapi.json
  format: json
  label: Dealogic Analytics Company API
  slug: dealogic-analytics-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-analytics-company-openapi.json
- filename: dealogic-analytics-sponsor-openapi.json
  format: json
  label: Dealogic Analytics Sponsor API
  slug: dealogic-analytics-sponsor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-analytics-sponsor-openapi.json
- filename: dealogic-reporting-openapi.json
  format: json
  label: Dealogic Reporting API
  slug: dealogic-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-reporting-openapi.json
- filename: dealogic-cortex-reporting-openapi.json
  format: json
  label: Cortex Reporting API
  slug: cortex-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-cortex-reporting-openapi.json
- filename: dealogic-iona-profiles-openapi.json
  format: json
  label: IONA Profiles API
  slug: iona-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-iona-profiles-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dealogic.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iongroup.com
  spf: true
hosts:
- cert_expires: Nov 12 01:53:08 2026 GMT
  host: www.dealogic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 14:32:09 2026 GMT
  host: iongroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: spac.analytics.dealogic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Dealogic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dealogic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dealogic
provider_slug: dealogic
slug: dealogic-domain-security
source_filename: dealogic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dealogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 01:53:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: iongroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 14:32:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: spac.analytics.dealogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dealogic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: iongroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/security/dealogic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Capital Markets
- Compliance
- Deal Management
- Debt Capital Markets
- Equity Capital Markets
- Finance
- Financial Data
- Investment Banking
- League Tables
- M&A
- OData
- Private Equity
- Reporting
- SPAC
- Syndicated Loans
---
