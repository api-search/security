---
api_specs:
- filename: australian-taxation-office-apiinfo-api-openapi.yml
  format: yaml
  label: Australian Taxation Office API Info API
  slug: australian-taxation-office-apiinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-apiinfo-api-openapi.yml
- filename: australian-taxation-office-combined-global-and-domestic-group-entity-tax-return-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Combined Global and Domestic Group Entity Tax Return API
  slug: australian-taxation-office-combined-global-and-domestic-group-entity-tax-return-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-combined-global-and-domestic-group-entity-tax-return-api-openapi.yml
- filename: australian-taxation-office-combined-global-and-domestic-minimum-tax-return-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Combined Global and Domestic Minimum Tax Return API
  slug: australian-taxation-office-combined-global-and-domestic-minimum-tax-return-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-combined-global-and-domestic-minimum-tax-return-api-openapi.yml
- filename: australian-taxation-office-get-payee-stapled-super-fund-for-receipt-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Get Payee Stapled Super Fund for Receipt API
  slug: australian-taxation-office-get-payee-stapled-super-fund-for-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-get-payee-stapled-super-fund-for-receipt-api-openapi.yml
- filename: australian-taxation-office-get-payment-reference-number-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Get Payment Reference Number API
  slug: australian-taxation-office-get-payment-reference-number-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-get-payment-reference-number-api-openapi.yml
- filename: australian-taxation-office-gst-property-settlement-date-confirmation-api-openapi.yml
  format: yaml
  label: Australian Taxation Office GST Property Settlement Date Confirmation API
  slug: australian-taxation-office-gst-property-settlement-date-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-gst-property-settlement-date-confirmation-api-openapi.yml
- filename: australian-taxation-office-gst-property-settlement-withholding-notification-api-openapi.yml
  format: yaml
  label: Australian Taxation Office GST Property Settlement Withholding Notification API
  slug: australian-taxation-office-gst-property-settlement-withholding-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-gst-property-settlement-withholding-notification-api-openapi.yml
- filename: australian-taxation-office-heartbeat-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Heartbeat API
  slug: australian-taxation-office-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-heartbeat-api-openapi.yml
- filename: australian-taxation-office-providers-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Providers API
  slug: australian-taxation-office-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-providers-api-openapi.yml
- filename: australian-taxation-office-register-a-new-software-application-instance-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Register a new software application instance API
  slug: australian-taxation-office-register-a-new-software-application-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-register-a-new-software-application-instance-api-openapi.yml
- filename: australian-taxation-office-request-stapled-super-fund-for-payee-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Request Stapled Super Fund for Payee API
  slug: australian-taxation-office-request-stapled-super-fund-for-payee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-request-stapled-super-fund-for-payee-api-openapi.yml
- filename: australian-taxation-office-spec-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Spec API
  slug: australian-taxation-office-spec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-spec-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ato.gov.au
  spf: true
hosts:
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: ato.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Australian Taxation Office Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australian Taxation Office, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Australian Taxation Office
provider_slug: australian-taxation-office
slug: australian-taxation-office-domain-security
source_filename: australian-taxation-office-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ato.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ato.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/security/australian-taxation-office-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Government
- Taxation
- Superannuation
- Australia
- Digital Service Providers
- Public Sector
---
