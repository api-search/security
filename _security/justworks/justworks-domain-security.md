---
api_specs:
- filename: justworks-members-api-openapi.yml
  format: yaml
  label: Justworks Members API
  slug: justworks-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-members-api-openapi.yml
- filename: justworks-company-api-openapi.yml
  format: yaml
  label: Justworks Company API
  slug: justworks-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-company-api-openapi.yml
- filename: justworks-payroll-api-openapi.yml
  format: yaml
  label: Justworks Payroll API
  slug: justworks-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-payroll-api-openapi.yml
- filename: justworks-deductions-api-openapi.yml
  format: yaml
  label: Justworks Deductions API
  slug: justworks-deductions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-deductions-api-openapi.yml
- filename: justworks-time-off-api-openapi.yml
  format: yaml
  label: Justworks Time Off API
  slug: justworks-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-time-off-api-openapi.yml
- filename: justworks-webhooks-api-openapi.yml
  format: yaml
  label: Justworks Webhooks API
  slug: justworks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-webhooks-api-openapi.yml
- filename: justworks-oauth-api-openapi.yml
  format: yaml
  label: Justworks OAuth API
  slug: justworks-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-oauth-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: justworks.com
  spf: true
hosts:
- cert_expires: Aug 25 12:01:04 2026 GMT
  host: www.justworks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 14:41:50 2026 GMT
  host: public-api.justworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Justworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Justworks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Justworks
provider_slug: justworks
slug: justworks-domain-security
source_filename: justworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.justworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 12:01:04 2026 GMT\n  hsts: false\n- host: public-api.justworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 14:41:50 2026 GMT\n  hsts: null\ndomains:\n- domain: justworks.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/security/justworks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- PEO
- Payroll
- HR
- Human Resources
- Benefits
- Health Insurance
- 401(k)
- Time Off
- Compliance
- Small Business
- Employer of Record
- HRIS
---
