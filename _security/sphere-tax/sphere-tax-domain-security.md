---
api_specs:
- filename: sphere-tax-openapi.yml
  format: yaml
  label: Sphere Tax Calculations API
  slug: sphere-tax-calculations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/openapi/sphere-tax-openapi.yml
- filename: sphere-tax-openapi.yml
  format: yaml
  label: Sphere Transactions Export API
  slug: sphere-transactions-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/openapi/sphere-tax-openapi.yml
- filename: sphere-tax-openapi.yml
  format: yaml
  label: Sphere Registrations and Filings API
  slug: sphere-registrations-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/openapi/sphere-tax-openapi.yml
- filename: sphere-tax-openapi.yml
  format: yaml
  label: Sphere Nexus Monitoring API
  slug: sphere-nexus-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/openapi/sphere-tax-openapi.yml
- filename: sphere-tax-openapi.yml
  format: yaml
  label: Sphere Exemptions API
  slug: sphere-exemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/openapi/sphere-tax-openapi.yml
- filename: sphere-tax-openapi.yml
  format: yaml
  label: Sphere Webhooks API
  slug: sphere-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/openapi/sphere-tax-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getsphere.com
  spf: true
hosts:
- cert_expires: Aug 16 07:42:13 2026 GMT
  host: www.getsphere.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 08:31:44 2026 GMT
  host: docs.getsphere.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: server.getsphere.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sphere Tax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sphere, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Sphere
provider_slug: sphere-tax
slug: sphere-tax-domain-security
source_filename: sphere-tax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getsphere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 07:42:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.getsphere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 08:31:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: server.getsphere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: getsphere.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/security/sphere-tax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Tax
- Sales Tax
- VAT
- GST
- Compliance
- FinTech
---
