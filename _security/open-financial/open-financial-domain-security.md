---
api_specs:
- filename: open-financial-accounts-api-openapi.yml
  format: yaml
  label: Open (open.money) Accounts API
  slug: open-financial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-accounts-api-openapi.yml
- filename: open-financial-constants-api-openapi.yml
  format: yaml
  label: Open (open.money) Constants API
  slug: open-financial-constants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-constants-api-openapi.yml
- filename: open-financial-events-api-openapi.yml
  format: yaml
  label: Open (open.money) Events API
  slug: open-financial-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-events-api-openapi.yml
- filename: open-financial-icp-api-openapi.yml
  format: yaml
  label: Open (open.money) Icp API
  slug: open-financial-icp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-icp-api-openapi.yml
- filename: open-financial-kycs-api-openapi.yml
  format: yaml
  label: Open (open.money) Kycs API
  slug: open-financial-kycs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-kycs-api-openapi.yml
- filename: open-financial-pg-api-openapi.yml
  format: yaml
  label: Open (open.money) Pg API
  slug: open-financial-pg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-pg-api-openapi.yml
- filename: open-financial-pg-settlements-api-openapi.yml
  format: yaml
  label: Open (open.money) Pg Settlements API
  slug: open-financial-pg-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-pg-settlements-api-openapi.yml
- filename: open-financial-refund-api-openapi.yml
  format: yaml
  label: Open (open.money) Refund API
  slug: open-financial-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-refund-api-openapi.yml
- filename: open-financial-transfers-api-openapi.yml
  format: yaml
  label: Open (open.money) Transfers API
  slug: open-financial-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-transfers-api-openapi.yml
- filename: open-financial-verifications-api-openapi.yml
  format: yaml
  label: Open (open.money) Verifications API
  slug: open-financial-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-verifications-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: open.money
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: zwitch.io
  spf: true
hosts:
- cert_expires: Dec  8 05:18:17 2026 GMT
  host: open.money
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 02:31:34 2026 GMT
  host: www.zwitch.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 00:04:25 2026 GMT
  host: developers.zwitch.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Open Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open (open.money), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Open (open.money)
provider_slug: open-financial
slug: open-financial-domain-security
source_filename: open-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 05:18:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.zwitch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 02:31:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.zwitch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 00:04:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: open.money\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zwitch.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/security/open-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Connected Banking
- Neobank
- Small Business
- Embedded Finance
- Banking as a Service
- Payments
- Payouts
- UPI
- Accounting
- Payroll
- Expense Management
- India
- Fintech
---
