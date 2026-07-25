---
api_specs:
- filename: upward-financial-accounts-api-openapi.yml
  format: yaml
  label: Upward Financial accounts API
  slug: upward-financial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-accounts-api-openapi.yml
- filename: upward-financial-auth-api-openapi.yml
  format: yaml
  label: Upward Financial auth API
  slug: upward-financial-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-auth-api-openapi.yml
- filename: upward-financial-billpayments-api-openapi.yml
  format: yaml
  label: Upward Financial billPayments API
  slug: upward-financial-billpayments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-billpayments-api-openapi.yml
- filename: upward-financial-billreporting-api-openapi.yml
  format: yaml
  label: Upward Financial billReporting API
  slug: upward-financial-billreporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-billreporting-api-openapi.yml
- filename: upward-financial-billswitch-api-openapi.yml
  format: yaml
  label: Upward Financial billSwitch API
  slug: upward-financial-billswitch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-billswitch-api-openapi.yml
- filename: upward-financial-cbaas-api-openapi.yml
  format: yaml
  label: Upward Financial cbaas API
  slug: upward-financial-cbaas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-cbaas-api-openapi.yml
- filename: upward-financial-consumers-api-openapi.yml
  format: yaml
  label: Upward Financial consumers API
  slug: upward-financial-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-consumers-api-openapi.yml
- filename: upward-financial-creditinsights-api-openapi.yml
  format: yaml
  label: Upward Financial creditInsights API
  slug: upward-financial-creditinsights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-creditinsights-api-openapi.yml
- filename: upward-financial-onboarding-api-openapi.yml
  format: yaml
  label: Upward Financial onboarding API
  slug: upward-financial-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-onboarding-api-openapi.yml
- filename: upward-financial-partners-api-openapi.yml
  format: yaml
  label: Upward Financial partners API
  slug: upward-financial-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-partners-api-openapi.yml
- filename: upward-financial-paymentcards-api-openapi.yml
  format: yaml
  label: Upward Financial paymentCards API
  slug: upward-financial-paymentcards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-paymentcards-api-openapi.yml
- filename: upward-financial-payments-api-openapi.yml
  format: yaml
  label: Upward Financial payments API
  slug: upward-financial-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-payments-api-openapi.yml
- filename: upward-financial-plaid-api-openapi.yml
  format: yaml
  label: Upward Financial plaid API
  slug: upward-financial-plaid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-plaid-api-openapi.yml
- filename: upward-financial-rewards-api-openapi.yml
  format: yaml
  label: Upward Financial rewards API
  slug: upward-financial-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-rewards-api-openapi.yml
- filename: upward-financial-simulations-api-openapi.yml
  format: yaml
  label: Upward Financial simulations API
  slug: upward-financial-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-simulations-api-openapi.yml
- filename: upward-financial-statements-api-openapi.yml
  format: yaml
  label: Upward Financial statements API
  slug: upward-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-statements-api-openapi.yml
- filename: upward-financial-webhooks-api-openapi.yml
  format: yaml
  label: Upward Financial webhooks API
  slug: upward-financial-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-webhooks-api-openapi.yml
description: Domain and transport security posture probed 2026-07-21. The production API and authorization hosts (api.upwardli.com, auth.upwardli.com) do not answer unauthenticated public HTTPS probes (connection timeouts), so no TLS data is recorded for them. The OpenAPI's servers[] entry is a placeholder (https://host.com) and is excluded; real hosts come from the documented environments page.
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: upwardli.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:spf.mandrillapp.com include:amazonses.com ~all
hosts:
- cert_expires: Aug 26 03:11:50 2026 GMT
  host: upwardli.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 18 22:16:46 2026 GMT
  host: www.upwardli.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 5 01:13:51 2026 GMT
  host: developers.upwardli.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 00:50:13 2026 GMT
  host: status.upwardli.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- host: api.upwardli.com
  https: null
  note: connection timeout - not publicly reachable
- host: auth.upwardli.com
  https: null
  note: connection timeout - not publicly reachable
kind: domain-security
layout: security
method: probed
name: Upward Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upward Financial, probed live across 6 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Upward Financial
provider_slug: upward-financial
slug: upward-financial-domain-security
source_filename: upward-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the Upwardli web, developer, status, API, and auth hosts\ndescription: >-\n  Domain and transport security posture probed 2026-07-21. The production API\n  and authorization hosts (api.upwardli.com, auth.upwardli.com) do not answer\n  unauthenticated public HTTPS probes (connection timeouts), so no TLS data is\n  recorded for them. The OpenAPI's servers[] entry is a placeholder\n  (https://host.com) and is excluded; real hosts come from the documented\n  environments page.\nhosts:\n- host: upwardli.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 26 03:11:50 2026 GMT\n  hsts: false\n- host: www.upwardli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 22:16:46 2026 GMT\n  hsts: false\n- host: developers.upwardli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 5 01:13:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n\
  \  hsts_preload: true\n- host: status.upwardli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 00:50:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n- host: api.upwardli.com\n  https: null\n  note: connection timeout - not publicly reachable\n- host: auth.upwardli.com\n  https: null\n  note: connection timeout - not publicly reachable\ndomains:\n- domain: upwardli.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: \"v=spf1 include:_spf.google.com include:spf.mandrillapp.com include:amazonses.com ~all\"\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/security/upward-financial-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- FinTech
- Credit
- Credit Building
- Payments
- Cards
- Embedded Finance
- Bill Pay
- Banking
- KYC
---
