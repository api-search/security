---
api_specs:
- filename: getting-started
  format: yaml
  label: NMI Payment API
  slug: nmi-payment-api
  spec_type: OpenAPI
  url: https://docs.nmi.com/reference/getting-started
- filename: getting-started
  format: yaml
  label: NMI Customer Vault API
  slug: nmi-customer-vault-api
  spec_type: OpenAPI
  url: https://docs.nmi.com/reference/getting-started
- filename: getting-started
  format: yaml
  label: NMI Recurring Billing API
  slug: nmi-recurring-billing-api
  spec_type: OpenAPI
  url: https://docs.nmi.com/reference/getting-started
- filename: getting-started
  format: yaml
  label: NMI Query API
  slug: nmi-query-api
  spec_type: OpenAPI
  url: https://docs.nmi.com/reference/getting-started
- filename: getting-started
  format: yaml
  label: NMI Merchant Onboarding API
  slug: nmi-merchant-onboarding-api
  spec_type: OpenAPI
  url: https://docs.nmi.com/reference/getting-started
- filename: getting-started
  format: yaml
  label: NMI Webhooks API
  slug: nmi-webhooks-api
  spec_type: OpenAPI
  url: https://docs.nmi.com/reference/getting-started
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nmi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: networkmerchants.com
  spf: true
hosts:
- cert_expires: Sep 12 00:27:41 2026 GMT
  host: docs.nmi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: secure.networkmerchants.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 23:40:09 2026 GMT
  host: support.nmi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nmi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NMI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NMI
provider_slug: nmi
slug: nmi-domain-security
source_filename: nmi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.nmi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 00:27:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: secure.networkmerchants.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.nmi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:40:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nmi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: networkmerchants.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nmi/refs/heads/main/security/nmi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- Payment Processing
- Tokenization
- Recurring Billing
- Customer Vault
- Fintech
- Embedded Payments
- Payment Facilitation
---
