---
api_specs:
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Payment Intents API
  slug: paymongo-payment-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Payment Methods API
  slug: paymongo-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Payments API
  slug: paymongo-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Sources API
  slug: paymongo-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Checkout Sessions API
  slug: paymongo-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Payment Links API
  slug: paymongo-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Customers API
  slug: paymongo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Refunds API
  slug: paymongo-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo QR Ph API
  slug: paymongo-qr-ph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Webhooks API
  slug: paymongo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Subscriptions & Plans API
  slug: paymongo-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Money Movement API
  slug: paymongo-money-movement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Forex API
  slug: paymongo-forex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Fraud Detection API
  slug: paymongo-fraud-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:caa-violations@paymongo.com"
  dmarc: true
  dmarc_note: p=quarantine; sp=quarantine; pct=25; rua/ruf mailto:dmarc-report@paymongo.com
  dmarc_policy: quarantine
  dnssec: false
  domain: paymongo.com
  spf: true
  spf_record: v=spf1 include:_spf.createsend.com include:_spf.google.com include:7079113.spf03.hubspotemail.net ~all
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: paymongo.com
  hsts: null
  https: true
  server: CloudFront
- auth_required: true
  cert_expires: Feb 20 23:59:59 2027 GMT
  host: api.paymongo.com
  hsts: null
  https: true
  probe_status: 401
- host: docs.paymongo.com
  https: true
  note: developers.paymongo.com issues a 301 redirect to docs.paymongo.com
kind: domain-security
layout: security
method: probed
name: Paymongo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayMongo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PayMongo
provider_slug: paymongo
slug: paymongo-domain-security
source_filename: paymongo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paymongo.com\n  https: true\n  server: CloudFront\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: null\n- host: api.paymongo.com\n  https: true\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  auth_required: true\n  probe_status: 401\n  hsts: null\n- host: docs.paymongo.com\n  https: true\n  note: developers.paymongo.com issues a 301 redirect to docs.paymongo.com\ndomains:\n- domain: paymongo.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:caa-violations@paymongo.com\"\n  spf: true\n  spf_record: v=spf1 include:_spf.createsend.com include:_spf.google.com include:7079113.spf03.hubspotemail.net ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_note: p=quarantine; sp=quarantine; pct=25; rua/ruf mailto:dmarc-report@paymongo.com\n\
  notes: >-\n  api.paymongo.com and paymongo.com both serve valid TLS certificates (expiry\n  Feb 20 2027) fronted by AWS CloudFront. api.paymongo.com/v1 returns HTTP 401\n  without credentials, confirming enforced authentication. A CAA record scopes\n  issuance to a defined set of CAs with an iodef violation contact. SPF and\n  DMARC (quarantine) are published. No HSTS header was observed on the probed\n  hosts at probe time, and no /.well-known/security.txt was found (HTTP 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/security/paymongo-domain-security.yml
summary_line: DMARC
tags:
- Payments
- FinTech
- Philippines
- Southeast Asia
- GCash
- E-Wallet
- Card Payments
---
