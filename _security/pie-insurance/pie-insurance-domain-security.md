---
api_specs:
- filename: pie-insurance-partner-api-openapi.yml
  format: yaml
  label: Pie Insurance Partner API
  slug: pie-insurance-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pie-insurance/refs/heads/main/openapi/pie-insurance-partner-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pieinsurance.com
  spf: true
hosts:
- cert_expires: Sep  8 14:42:33 2026 GMT
  host: www.pieinsurance.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: api.post-prod.pieinsurance.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pie Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pie Insurance, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pie Insurance
provider_slug: pie-insurance
slug: pie-insurance-domain-security
source_filename: pie-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pieinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 14:42:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.post-prod.pieinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: pieinsurance.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pie-insurance/refs/heads/main/security/pie-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- Workers Compensation
- Small Business
- Commercial Insurance
- Business Owners Policy
- Commercial Auto
- General Liability
- Professional Liability
- Agency Portal
- Partner API
- Quoting
- Binding
---
