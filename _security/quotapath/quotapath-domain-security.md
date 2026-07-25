---
api_specs:
- filename: quotapath-data-api-openapi.yml
  format: yaml
  label: QuotaPath data API
  slug: quotapath-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quotapath/refs/heads/main/openapi/quotapath-data-api-openapi.yml
- filename: quotapath-deal-api-openapi.yml
  format: yaml
  label: QuotaPath deal API
  slug: quotapath-deal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quotapath/refs/heads/main/openapi/quotapath-deal-api-openapi.yml
- filename: quotapath-path-api-openapi.yml
  format: yaml
  label: QuotaPath path API
  slug: quotapath-path-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quotapath/refs/heads/main/openapi/quotapath-path-api-openapi.yml
- filename: quotapath-payout-api-openapi.yml
  format: yaml
  label: QuotaPath payout API
  slug: quotapath-payout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quotapath/refs/heads/main/openapi/quotapath-payout-api-openapi.yml
- filename: quotapath-plan-api-openapi.yml
  format: yaml
  label: QuotaPath plan API
  slug: quotapath-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quotapath/refs/heads/main/openapi/quotapath-plan-api-openapi.yml
- filename: quotapath-team-api-openapi.yml
  format: yaml
  label: QuotaPath team API
  slug: quotapath-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quotapath/refs/heads/main/openapi/quotapath-team-api-openapi.yml
- filename: quotapath-user-api-openapi.yml
  format: yaml
  label: QuotaPath user API
  slug: quotapath-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quotapath/refs/heads/main/openapi/quotapath-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quotapath.com
  spf: true
hosts:
- cert_expires: Sep 25 09:49:33 2026 GMT
  host: www.quotapath.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 08:46:04 2026 GMT
  host: api.quotapath.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quotapath Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QuotaPath, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: QuotaPath
provider_slug: quotapath
slug: quotapath-domain-security
source_filename: quotapath-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quotapath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 09:49:33 2026 GMT\n  hsts: false\n- host: api.quotapath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:46:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quotapath.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quotapath/refs/heads/main/security/quotapath-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sales Commissions
- Compensation Management
- Sales Operations
- Revenue Operations
- Finance
- Payouts
- CRM Integration
- Payroll
---
