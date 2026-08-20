---
api_specs:
- filename: keycorp-commercial-accounts-reporting-openapi.yml
  format: yaml
  label: KeyBank Account Information API
  slug: account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-commercial-accounts-reporting-openapi.yml
- filename: keycorp-ach-originations-openapi.yml
  format: yaml
  label: KeyBank ACH Origination API
  slug: ach-origination-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-ach-originations-openapi.yml
- filename: keycorp-rtp-wire-payments-openapi.yml
  format: yaml
  label: KeyBank Wire Transfer API
  slug: wire-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-rtp-wire-payments-openapi.yml
- filename: keycorp-rtp-wire-payments-openapi.yml
  format: yaml
  label: KeyBank RTP Send Payment API
  slug: rtp-send-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-rtp-wire-payments-openapi.yml
- filename: keycorp-account-validation-openapi.yml
  format: yaml
  label: KeyBank Account Validation API
  slug: account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-account-validation-openapi.yml
- filename: keycorp-ach-inquiry-openapi.yml
  format: yaml
  label: KeyBank ACH Inquiry API
  slug: ach-inquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-ach-inquiry-openapi.yml
- filename: keycorp-wire-inquiry-openapi.yml
  format: yaml
  label: KeyBank Wire Inquiry API
  slug: wire-inquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-wire-inquiry-openapi.yml
- filename: keycorp-rtp-inquiry-openapi.yml
  format: yaml
  label: KeyBank RTP Inquiry API
  slug: rtp-inquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-rtp-inquiry-openapi.yml
- filename: keycorp-check-services-openapi.yml
  format: yaml
  label: KeyBank Check Services API
  slug: check-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-check-services-openapi.yml
- filename: keycorp-webhooks-openapi.yml
  format: yaml
  label: KeyBank Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-webhooks-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 issuewild "pki.goog"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: key.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: keycorp.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.key.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: www.keycorp.com
  https: false
- cert_expires: Aug  8 23:59:59 2026 GMT
  host: developer.key.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keycorp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KeyCorp, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: KeyCorp
provider_slug: keycorp
slug: keycorp-domain-security
source_filename: keycorp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.key.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\n- host: www.keycorp.com\n  https: false\n- host: developer.key.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: key.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: keycorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/security/keycorp-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Banking
- Commercial Banking
- Financial-Services
- Fortune 500
- Payments
- United States
- Super-Regional Bank
- Treasury Management
- Embedded Banking
- ACH
- Real-Time Payments
- Wire Transfer
---
