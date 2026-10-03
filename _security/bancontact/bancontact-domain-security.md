---
api_specs:
- filename: bancontact-callback-to-merchants-api-openapi.yml
  format: yaml
  label: Bancontact Callback to Merchants API
  slug: bancontact-callback-to-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bancontact/refs/heads/main/openapi/bancontact-callback-to-merchants-api-openapi.yml
- filename: bancontact-merchant-acknowledge-api-openapi.yml
  format: yaml
  label: Bancontact Merchant Acknowledge API
  slug: bancontact-merchant-acknowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bancontact/refs/heads/main/openapi/bancontact-merchant-acknowledge-api-openapi.yml
- filename: bancontact-merchant-endpoints-api-openapi.yml
  format: yaml
  label: Bancontact Merchant Endpoints API
  slug: bancontact-merchant-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bancontact/refs/heads/main/openapi/bancontact-merchant-endpoints-api-openapi.yml
- filename: bancontact-payments-api-openapi.yml
  format: yaml
  label: Bancontact Payments API
  slug: bancontact-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bancontact/refs/heads/main/openapi/bancontact-payments-api-openapi.yml
- filename: bancontact-payoutlist-api-openapi.yml
  format: yaml
  label: Bancontact Payout List API
  slug: bancontact-payoutlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bancontact/refs/heads/main/openapi/bancontact-payoutlist-api-openapi.yml
- filename: bancontact-payoutpayments-api-openapi.yml
  format: yaml
  label: Bancontact Payout Payments API
  slug: bancontact-payoutpayments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bancontact/refs/heads/main/openapi/bancontact-payoutpayments-api-openapi.yml
- filename: bancontact-payoutrefunds-api-openapi.yml
  format: yaml
  label: Bancontact Payout Refunds API
  slug: bancontact-payoutrefunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bancontact/refs/heads/main/openapi/bancontact-payoutrefunds-api-openapi.yml
- filename: bancontact-refunds-api-openapi.yml
  format: yaml
  label: Bancontact Refunds API
  slug: bancontact-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bancontact/refs/heads/main/openapi/bancontact-refunds-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bancontact.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: bancontactpro.com
  spf: true
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: www.bancontact.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 05:09:40 2026 GMT
  host: docs.bancontactpro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: merchant.api.bancontact.net
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Bancontact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bancontact, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bancontact
provider_slug: bancontact
slug: bancontact-domain-security
source_filename: bancontact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bancontact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: false\n- host: docs.bancontactpro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 05:09:40 2026 GMT\n  hsts: false\n- host: merchant.api.bancontact.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bancontact.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bancontactpro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bancontact/refs/heads/main/security/bancontact-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Banking
- Belgium
- Debit Cards
- E-Commerce
- Fintech
- Payments
- QR Codes
- Refunds
- Reconciliation
- Mobile Payments
---
