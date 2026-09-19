---
api_specs:
- filename: dealogic-admin-api-openapi.yml
  format: yaml
  label: Dealogic Admin API
  slug: dealogic-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-admin-api-openapi.yml
- filename: dealogic-data-api-openapi.yml
  format: yaml
  label: Dealogic Data API
  slug: dealogic-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-data-api-openapi.yml
- filename: dealogic-dcmdeal-api-openapi.yml
  format: yaml
  label: Dealogic Dcm Deal API
  slug: dealogic-dcmdeal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-dcmdeal-api-openapi.yml
- filename: dealogic-entity-navigation-api-openapi.yml
  format: yaml
  label: Dealogic Entity Navigation API
  slug: dealogic-entity-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-entity-navigation-api-openapi.yml
- filename: dealogic-levfinmarketupdate-api-openapi.yml
  format: yaml
  label: Dealogic Levfin Market Update API
  slug: dealogic-levfinmarketupdate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-levfinmarketupdate-api-openapi.yml
- filename: dealogic-loandeal-api-openapi.yml
  format: yaml
  label: Dealogic Loan Deal API
  slug: dealogic-loandeal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-loandeal-api-openapi.yml
- filename: dealogic-organizationspacprofile-api-openapi.yml
  format: yaml
  label: Dealogic Organization Spac Profile API
  slug: dealogic-organizationspacprofile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-organizationspacprofile-api-openapi.yml
- filename: dealogic-related-entities-api-openapi.yml
  format: yaml
  label: Dealogic Related Entities API
  slug: dealogic-related-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-related-entities-api-openapi.yml
- filename: dealogic-reportdata-api-openapi.yml
  format: yaml
  label: Dealogic Report Data API
  slug: dealogic-reportdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-reportdata-api-openapi.yml
- filename: dealogic-root-entity-api-openapi.yml
  format: yaml
  label: Dealogic Root Entity API
  slug: dealogic-root-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-root-entity-api-openapi.yml
- filename: dealogic-spac-admin-api-openapi.yml
  format: yaml
  label: Dealogic Spac Admin API
  slug: dealogic-spac-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-spac-admin-api-openapi.yml
- filename: dealogic-spac-reader-api-openapi.yml
  format: yaml
  label: Dealogic Spac Reader API
  slug: dealogic-spac-reader-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-spac-reader-api-openapi.yml
- filename: dealogic-spac-writer-api-openapi.yml
  format: yaml
  label: Dealogic Spac Writer API
  slug: dealogic-spac-writer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-spac-writer-api-openapi.yml
- filename: dealogic-test-api-openapi.yml
  format: yaml
  label: Dealogic Test API
  slug: dealogic-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-test-api-openapi.yml
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
