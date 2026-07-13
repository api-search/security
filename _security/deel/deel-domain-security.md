---
api_specs:
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel People API
  slug: deel-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Organizations API
  slug: deel-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Contracts API
  slug: deel-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Time Off API
  slug: deel-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Time Tracking API
  slug: deel-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Payroll API
  slug: deel-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Invoices API
  slug: deel-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Expenses API
  slug: deel-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel EOR API
  slug: deel-eor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Background Checks API
  slug: deel-background-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Immigration API
  slug: deel-immigration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel IT API
  slug: deel-it-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel SCIM API
  slug: deel-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel ATS API
  slug: deel-ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Accounting API
  slug: deel-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Lookups API
  slug: deel-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Webhooks API
  slug: deel-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel OAuth & Apps API
  slug: deel-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel MCP Server
  slug: deel-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:security@letsdeel.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: deel.com
  spf: true
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: letsdeel.com
  spf: true
hosts:
- cert_expires: Aug 25 11:52:29 2026 GMT
  host: www.deel.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 00:38:22 2026 GMT
  host: api.letsdeel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api-staging.letsdeel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deel, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Deel
provider_slug: deel
slug: deel-domain-security
source_filename: deel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 11:52:29 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.letsdeel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 00:38:22 2026 GMT\n  hsts: null\n- host: api-staging.letsdeel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: deel.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:security@letsdeel.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: letsdeel.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\
  \n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/security/deel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- HR
- Payroll
- Global Hiring
- EOR
- Contractors
- Compliance
- SCIM
---
