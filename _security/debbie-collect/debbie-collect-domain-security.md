---
api_specs:
- filename: debbie-collect-billing-api-openapi.yml
  format: yaml
  label: Debbie Collect Billing API
  slug: debbie-collect-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-billing-api-openapi.yml
- filename: debbie-collect-case-vouchers-api-openapi.yml
  format: yaml
  label: Debbie Collect Case Vouchers API
  slug: debbie-collect-case-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-case-vouchers-api-openapi.yml
- filename: debbie-collect-cases-api-openapi.yml
  format: yaml
  label: Debbie Collect Cases API
  slug: debbie-collect-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-cases-api-openapi.yml
- filename: debbie-collect-creditors-api-openapi.yml
  format: yaml
  label: Debbie Collect Creditors API
  slug: debbie-collect-creditors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-creditors-api-openapi.yml
- filename: debbie-collect-customers-api-openapi.yml
  format: yaml
  label: Debbie Collect Customers API
  slug: debbie-collect-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-customers-api-openapi.yml
- filename: debbie-collect-files-api-openapi.yml
  format: yaml
  label: Debbie Collect Files API
  slug: debbie-collect-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-files-api-openapi.yml
- filename: debbie-collect-payments-api-openapi.yml
  format: yaml
  label: Debbie Collect Payments API
  slug: debbie-collect-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-payments-api-openapi.yml
- filename: debbie-collect-properties-api-openapi.yml
  format: yaml
  label: Debbie Collect Properties API
  slug: debbie-collect-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-properties-api-openapi.yml
- filename: debbie-collect-updates-api-openapi.yml
  format: yaml
  label: Debbie Collect Updates API
  slug: debbie-collect-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-updates-api-openapi.yml
- filename: debbie-collect-webhooks-api-openapi.yml
  format: yaml
  label: Debbie Collect Webhooks API
  slug: debbie-collect-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/openapi/debbie-collect-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: debbiecollect.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: debbie.dk
  spf: true
hosts:
- cert_expires: Sep 10 06:16:46 2026 GMT
  host: debbiecollect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 06:03:14 2026 GMT
  host: documentation.debbiecollect.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.debbie.dk
  https: false
kind: domain-security
layout: security
method: probed
name: Debbie Collect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Debbie Collect, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Debbie Collect
provider_slug: debbie-collect
slug: debbie-collect-domain-security
source_filename: debbie-collect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: debbiecollect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:16:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.debbiecollect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 06:03:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.debbie.dk\n  https: false\ndomains:\n- domain: debbiecollect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: debbie.dk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debbie-collect/refs/heads/main/security/debbie-collect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounts Receivable
- Collections
- Debt Collection
- FinTech
- Payments
- SaaS
---
