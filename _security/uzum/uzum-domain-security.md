---
api_specs:
- filename: uzum-api-mfo-api-openapi.yml
  format: yaml
  label: Uzum API MFO API
  slug: uzum-api-mfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-api-mfo-api-openapi.yml
- filename: uzum-auxiliary-methods-api-openapi.yml
  format: yaml
  label: Uzum Auxiliary Methods API
  slug: uzum-auxiliary-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-auxiliary-methods-api-openapi.yml
- filename: uzum-back-to-back-payment-api-openapi.yml
  format: yaml
  label: Uzum Back-to-back Payment API
  slug: uzum-back-to-back-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-back-to-back-payment-api-openapi.yml
- filename: uzum-check-service-status-api-openapi.yml
  format: yaml
  label: Uzum Check Service Status API
  slug: uzum-check-service-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-check-service-status-api-openapi.yml
- filename: uzum-common-methods-api-openapi.yml
  format: yaml
  label: Uzum Common methods API
  slug: uzum-common-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-common-methods-api-openapi.yml
- filename: uzum-cross-border-payments-api-openapi.yml
  format: yaml
  label: Uzum Cross-border payments API
  slug: uzum-cross-border-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-cross-border-payments-api-openapi.yml
- filename: uzum-fiscalization-api-openapi.yml
  format: yaml
  label: Uzum Fiscalization API
  slug: uzum-fiscalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-fiscalization-api-openapi.yml
- filename: uzum-from-uzbekistan-api-openapi.yml
  format: yaml
  label: Uzum From Uzbekistan API
  slug: uzum-from-uzbekistan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-from-uzbekistan-api-openapi.yml
- filename: uzum-information-retrieval-api-openapi.yml
  format: yaml
  label: Uzum Information retrieval API
  slug: uzum-information-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-information-retrieval-api-openapi.yml
- filename: uzum-managing-credit-cards-bindings-api-openapi.yml
  format: yaml
  label: Uzum Managing Credit Cards Bindings API
  slug: uzum-managing-credit-cards-bindings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-managing-credit-cards-bindings-api-openapi.yml
- filename: uzum-methods-api-openapi.yml
  format: yaml
  label: Uzum Methods API
  slug: uzum-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-methods-api-openapi.yml
- filename: uzum-one-step-payment-api-openapi.yml
  format: yaml
  label: Uzum One-Step Payment API
  slug: uzum-one-step-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-one-step-payment-api-openapi.yml
- filename: uzum-partner-api-openapi.yml
  format: yaml
  label: Uzum Partner API
  slug: uzum-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-partner-api-openapi.yml
- filename: uzum-submit-qr-code-payment-receipt-to-tax-authorities-api-openapi.yml
  format: yaml
  label: Uzum Submit QR Code Payment Receipt to Tax Authorities API
  slug: uzum-submit-qr-code-payment-receipt-to-tax-authorities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-submit-qr-code-payment-receipt-to-tax-authorities-api-openapi.yml
- filename: uzum-to-uzbekistan-api-openapi.yml
  format: yaml
  label: Uzum To Uzbekistan API
  slug: uzum-to-uzbekistan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-to-uzbekistan-api-openapi.yml
- filename: uzum-transfer-process-api-openapi.yml
  format: yaml
  label: Uzum Transfer process API
  slug: uzum-transfer-process-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-transfer-process-api-openapi.yml
- filename: uzum-two-step-payment-api-openapi.yml
  format: yaml
  label: Uzum Two-Step Payment API
  slug: uzum-two-step-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-two-step-payment-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uzum.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uzumbank.uz
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: uzum.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: developer.uzumbank.uz
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: crossborder.transfer.uz
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Uzum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uzum, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Uzum
provider_slug: uzum
slug: uzum-domain-security
source_filename: uzum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uzum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: false\n- host: developer.uzumbank.uz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: crossborder.transfer.uz\n  https: false\ndomains:\n- domain: uzum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: uzumbank.uz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/security/uzum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Banking
- Financial-Services
- E-Commerce
- Marketplace
- Money Transfer
- Remittances
- Buy Now Pay Later
- Acquiring
- QR Payments
- Fiscalization
- Banking as a Service
- Uzbekistan
- Central Asia
---
