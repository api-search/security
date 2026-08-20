---
api_specs:
- filename: nuvei-payments-api-openapi.yml
  format: yaml
  label: Nuvei Payments API
  slug: nuvei-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-payments-api-openapi.yml
- filename: nuvei-payouts-api-openapi.yml
  format: yaml
  label: Nuvei Payouts API
  slug: nuvei-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-payouts-api-openapi.yml
- filename: nuvei-user-payment-options-api-openapi.yml
  format: yaml
  label: Nuvei User Payment Options API
  slug: nuvei-user-payment-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-user-payment-options-api-openapi.yml
- filename: nuvei-3ds-api-openapi.yml
  format: yaml
  label: Nuvei 3DS API
  slug: nuvei-3ds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-3ds-api-openapi.yml
- filename: nuvei-dcc-api-openapi.yml
  format: yaml
  label: Nuvei DCC API
  slug: nuvei-dcc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-dcc-api-openapi.yml
- filename: nuvei-dmn-asyncapi.yml
  format: yaml
  label: Nuvei Direct Merchant Notifications (DMN)
  slug: nuvei-webhooks-dmn
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/asyncapi/nuvei-dmn-asyncapi.yml
- filename: nuvei-financial-operations-api-openapi.yml
  format: yaml
  label: Nuvei Financial Operations API
  slug: nuvei-financial-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-financial-operations-api-openapi.yml
- filename: nuvei-merchant-api-openapi.yml
  format: yaml
  label: Nuvei Merchant API
  slug: nuvei-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-merchant-api-openapi.yml
- filename: nuvei-orders-api-openapi.yml
  format: yaml
  label: Nuvei Orders API
  slug: nuvei-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-orders-api-openapi.yml
- filename: nuvei-sessions-api-openapi.yml
  format: yaml
  label: Nuvei Sessions API
  slug: nuvei-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-sessions-api-openapi.yml
- filename: nuvei-status-api-openapi.yml
  format: yaml
  label: Nuvei Status API
  slug: nuvei-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nuvei.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: safecharge.com
  spf: true
hosts:
- cert_expires: Aug 19 23:02:10 2026 GMT
  host: docs.nuvei.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: secure.safecharge.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: ppp-test.nuvei.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nuvei Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuvei, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nuvei
provider_slug: nuvei
slug: nuvei-domain-security
source_filename: nuvei-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.nuvei.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:02:10 2026 GMT\n  hsts: false\n- host: secure.safecharge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: false\n- host: ppp-test.nuvei.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nuvei.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: safecharge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/security/nuvei-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Payment Processing
- Payment Gateway
- Acquiring
- Payouts
- Alternative Payment Methods
- Fraud
- Risk
- Currency Conversion
- iGaming
- E-Commerce
- Fintech
---
