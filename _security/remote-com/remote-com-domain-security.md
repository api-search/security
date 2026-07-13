---
api_specs:
- filename: remote-companies-api-openapi.yml
  format: yaml
  label: Remote Companies API
  slug: remote-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-companies-api-openapi.yml
- filename: remote-employments-api-openapi.yml
  format: yaml
  label: Remote Employments API
  slug: remote-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-employments-api-openapi.yml
- filename: remote-contractors-api-openapi.yml
  format: yaml
  label: Remote Contractors API
  slug: remote-contractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-contractors-api-openapi.yml
- filename: remote-payroll-billing-api-openapi.yml
  format: yaml
  label: Remote Payroll and Billing API
  slug: remote-payroll-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-payroll-billing-api-openapi.yml
- filename: remote-time-attendance-api-openapi.yml
  format: yaml
  label: Remote Time and Attendance API
  slug: remote-time-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-time-attendance-api-openapi.yml
- filename: remote-benefits-api-openapi.yml
  format: yaml
  label: Remote Benefits API
  slug: remote-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-benefits-api-openapi.yml
- filename: remote-files-api-openapi.yml
  format: yaml
  label: Remote Files and Custom Fields API
  slug: remote-files-and-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-files-api-openapi.yml
- filename: remote-oauth-api-openapi.yml
  format: yaml
  label: Remote OAuth 2.0 API
  slug: remote-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-oauth-api-openapi.yml
- filename: remote-webhooks-asyncapi.yml
  format: yaml
  label: Remote Webhooks
  slug: remote-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/asyncapi/remote-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:sre-team@remote.com"
  - 0 issue "amazontrust.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: remote.com
  spf: true
hosts:
- cert_expires: Sep 15 07:37:04 2026 GMT
  host: remote.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 04:02:46 2026 GMT
  host: developer.remote.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: gateway.remote.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Remote Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Remote, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Remote
provider_slug: remote-com
slug: remote-com-domain-security
source_filename: remote-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: remote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:37:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.remote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 04:02:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.remote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: remote.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:sre-team@remote.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/security/remote-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Global Payroll
- EOR
- Contractor Management
- Contractor of Record
- PEO
- HRIS
- Recruiting
- Benefits
- Employment
- HR
- Compliance
- Workforce
- MCP
- AI Agents
---
