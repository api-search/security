---
api_specs:
- filename: avalara-avatax-rest-openapi.yml
  format: yaml
  label: AvaTax APIs
  slug: avatax-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-avatax-rest-openapi.yml
- filename: avalara-communications-openapi.yml
  format: yaml
  label: Communications Tax API
  slug: communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-communications-openapi.yml
- filename: avalara-excise-openapi.yml
  format: yaml
  label: Excise Platform API
  slug: excise-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-excise-openapi.yml
- filename: avalara-item-classification-openapi.yml
  format: yaml
  label: Item Classification API
  slug: item-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-item-classification-openapi.yml
- filename: avalara-avatax-brazil-openapi.yml
  format: yaml
  label: AvaTax Brazil API
  slug: avatax-brazil-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-avatax-brazil-openapi.yml
- filename: avalara-vat-reporting-openapi.yml
  format: yaml
  label: VAT Reporting API
  slug: vat-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-vat-reporting-openapi.yml
- filename: avalara-mylodgetax-openapi.yml
  format: yaml
  label: MyLodgeTax API
  slug: mylodgetax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-mylodgetax-openapi.yml
- filename: avalara-certcapture-openapi.yml
  format: yaml
  label: CertCapture API
  slug: certcapture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-certcapture-openapi.yml
- filename: avalara-e-invoicing-openapi.yml
  format: yaml
  label: E-Invoicing REST API
  slug: e-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-e-invoicing-openapi.yml
- filename: avalara-activation-service-openapi.yml
  format: yaml
  label: Activation Service API
  slug: activation-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-activation-service-openapi.yml
- filename: avalara-business-openapi.yml
  format: yaml
  label: Avalara Business API
  slug: business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-business-openapi.yml
- filename: avalara-portal-oauth-openapi.yml
  format: yaml
  label: Portal OAuth API
  slug: portal-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-portal-oauth-openapi.yml
- filename: avalara-shared-company-service-openapi.yml
  format: yaml
  label: Shared Company Service API
  slug: shared-company-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-shared-company-service-openapi.yml
- filename: avalara-hs-code-classification-openapi.yml
  format: yaml
  label: Automated Tariff Code Classification API
  slug: hs-code-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-hs-code-classification-openapi.yml
- filename: avalara-1099-w9-openapi.yml
  format: yaml
  label: 1099 & W-9 API
  slug: 1099-w9-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-1099-w9-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: avalara.com
  spf: true
hosts:
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: developer.avalara.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: api.avalara.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: api.sbx.avalara.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Avalara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avalara, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Avalara
provider_slug: avalara
slug: avalara-domain-security
source_filename: avalara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.avalara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.avalara.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: null\n- host: api.sbx.avalara.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: avalara.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/security/avalara-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Taxes
---
