---
api_specs:
- filename: notch-financial-openapi.yml
  format: yaml
  label: Notch Invoices API
  slug: invoices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-openapi.yml
- filename: notch-financial-openapi.yml
  format: yaml
  label: Notch Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-openapi.yml
- filename: notch-financial-openapi.yml
  format: yaml
  label: Notch Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-openapi.yml
- filename: notch-financial-openapi.yml
  format: yaml
  label: Notch Payment Methods API
  slug: payment-methods
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-openapi.yml
- filename: notch-financial-openapi.yml
  format: yaml
  label: Notch Bank Accounts API
  slug: bank-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-openapi.yml
- filename: notch-financial-openapi.yml
  format: yaml
  label: Notch Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: notch.financial
  spf: true
hosts:
- cert_expires: Sep 18 02:22:49 2026 GMT
  host: www.notch.financial
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.notch.financial
  https: false
kind: domain-security
layout: security
method: probed
name: Notch Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Notch, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Notch
provider_slug: notch-financial
slug: notch-financial-domain-security
source_filename: notch-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.notch.financial\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 02:22:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.notch.financial\n  https: false\ndomains:\n- domain: notch.financial\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/security/notch-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Accounts Receivable
- Accounts Payable
- B2B Payments
- Invoicing
- FinTech
---
