---
api_specs:
- filename: xero-accounting-openapi.yml
  format: yaml
  label: Xero Accounting API
  slug: xero-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-accounting-openapi.yml
- filename: xero-assets-openapi.yml
  format: yaml
  label: Xero Assets API
  slug: xero-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-assets-openapi.yml
- filename: xero-bankfeeds-openapi.yml
  format: yaml
  label: Xero Bank Feeds API
  slug: xero-bank-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-bankfeeds-openapi.yml
- filename: xero-finance-openapi.yml
  format: yaml
  label: Xero Finance API
  slug: xero-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-finance-openapi.yml
- filename: xero-identity-openapi.yml
  format: yaml
  label: Xero Identity API
  slug: xero-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-identity-openapi.yml
- filename: xero-payroll-au-openapi.yml
  format: yaml
  label: Xero Payroll Australia API
  slug: xero-payroll-australia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payroll-au-openapi.yml
- filename: xero-payroll-nz-openapi.yml
  format: yaml
  label: Xero Payroll New Zealand API
  slug: xero-payroll-new-zealand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payroll-nz-openapi.yml
- filename: xero-payroll-uk-openapi.yml
  format: yaml
  label: Xero Payroll United Kingdom API
  slug: xero-payroll-united-kingdom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payroll-uk-openapi.yml
- filename: xero-projects-openapi.yml
  format: yaml
  label: Xero Projects API
  slug: xero-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-projects-openapi.yml
- filename: xero-files-openapi.yml
  format: yaml
  label: Xero Files API
  slug: xero-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-files-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xero.com
  spf: true
hosts:
- cert_expires: Aug  2 22:00:00 2026 GMT
  host: developer.xero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: api.xero.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: identity.xero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xero, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Xero
provider_slug: xero
slug: xero-domain-security
source_filename: xero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.xero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 22:00:00 2026 GMT\n  hsts: false\n- host: api.xero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\n- host: identity.xero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: xero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/security/xero-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Accounting
- Bank Feeds
- Finance
- Financial Services
- Invoicing
- Payroll
- Small Business
---
