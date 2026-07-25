---
api_specs:
- filename: xero-accounting-api-openapi.yml
  format: yaml
  label: Xero Accounting API
  slug: xero-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-accounting-api-openapi.yml
- filename: xero-asset-api-openapi.yml
  format: yaml
  label: Xero Asset API
  slug: xero-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-asset-api-openapi.yml
- filename: xero-bankfeeds-api-openapi.yml
  format: yaml
  label: Xero BankFeeds API
  slug: xero-bankfeeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-bankfeeds-api-openapi.yml
- filename: xero-files-api-openapi.yml
  format: yaml
  label: Xero Files API
  slug: xero-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-files-api-openapi.yml
- filename: xero-finance-api-openapi.yml
  format: yaml
  label: Xero Finance API
  slug: xero-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-finance-api-openapi.yml
- filename: xero-identity-api-openapi.yml
  format: yaml
  label: Xero Identity API
  slug: xero-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-identity-api-openapi.yml
- filename: xero-payrollau-api-openapi.yml
  format: yaml
  label: Xero PayrollAu API
  slug: xero-payrollau-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payrollau-api-openapi.yml
- filename: xero-payrollnz-api-openapi.yml
  format: yaml
  label: Xero PayrollNz API
  slug: xero-payrollnz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payrollnz-api-openapi.yml
- filename: xero-payrolluk-api-openapi.yml
  format: yaml
  label: Xero PayrollUk API
  slug: xero-payrolluk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payrolluk-api-openapi.yml
- filename: xero-project-api-openapi.yml
  format: yaml
  label: Xero Project API
  slug: xero-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-project-api-openapi.yml
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
