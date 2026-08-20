---
api_specs:
- filename: bakkt-accounts-api-openapi.yml
  format: yaml
  label: Bakkt Accounts API
  slug: bakkt-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-accounts-api-openapi.yml
- filename: bakkt-authorization-api-openapi.yml
  format: yaml
  label: Bakkt Authorization API
  slug: bakkt-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-authorization-api-openapi.yml
- filename: bakkt-block-trade-allocate-api-openapi.yml
  format: yaml
  label: Bakkt Block Trade & Allocate API
  slug: bakkt-block-trade-allocate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-block-trade-allocate-api-openapi.yml
- filename: bakkt-configuration-and-status-api-openapi.yml
  format: yaml
  label: Bakkt Configuration and Status API
  slug: bakkt-configuration-and-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-configuration-and-status-api-openapi.yml
- filename: bakkt-currency-onboarding-api-openapi.yml
  format: yaml
  label: Bakkt Currency Onboarding API
  slug: bakkt-currency-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-currency-onboarding-api-openapi.yml
- filename: bakkt-documents-api-openapi.yml
  format: yaml
  label: Bakkt Documents API
  slug: bakkt-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-documents-api-openapi.yml
- filename: bakkt-fiat-onboarding-api-openapi.yml
  format: yaml
  label: Bakkt Fiat Onboarding API
  slug: bakkt-fiat-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-fiat-onboarding-api-openapi.yml
- filename: bakkt-gift-api-openapi.yml
  format: yaml
  label: Bakkt Gift API
  slug: bakkt-gift-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-gift-api-openapi.yml
- filename: bakkt-instruments-api-openapi.yml
  format: yaml
  label: Bakkt Instruments API
  slug: bakkt-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-instruments-api-openapi.yml
- filename: bakkt-jurisdictions-api-openapi.yml
  format: yaml
  label: Bakkt Jurisdictions API
  slug: bakkt-jurisdictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-jurisdictions-api-openapi.yml
- filename: bakkt-orders-api-openapi.yml
  format: yaml
  label: Bakkt Orders API
  slug: bakkt-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-orders-api-openapi.yml
- filename: bakkt-partner-connectivity-api-openapi.yml
  format: yaml
  label: Bakkt Partner Connectivity API
  slug: bakkt-partner-connectivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-partner-connectivity-api-openapi.yml
- filename: bakkt-partner-party-funding-api-openapi.yml
  format: yaml
  label: Bakkt Partner Party Funding API
  slug: bakkt-partner-party-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-partner-party-funding-api-openapi.yml
- filename: bakkt-partner-party-kyc-api-openapi.yml
  format: yaml
  label: Bakkt Partner Party Kyc API
  slug: bakkt-partner-party-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-partner-party-kyc-api-openapi.yml
- filename: bakkt-partner-party-linking-api-openapi.yml
  format: yaml
  label: Bakkt Partner Party Linking API
  slug: bakkt-partner-party-linking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-partner-party-linking-api-openapi.yml
- filename: bakkt-positions-api-openapi.yml
  format: yaml
  label: Bakkt Positions API
  slug: bakkt-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-positions-api-openapi.yml
- filename: bakkt-transfers-api-openapi.yml
  format: yaml
  label: Bakkt Transfers API
  slug: bakkt-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-transfers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bakkt.com
  spf: true
hosts:
- cert_expires: Oct  6 13:18:19 2026 GMT
  host: bakkt.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bakkt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bakkt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bakkt
provider_slug: bakkt
slug: bakkt-domain-security
source_filename: bakkt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bakkt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 13:18:19 2026 GMT\n  hsts: false\ndomains:\n- domain: bakkt.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/security/bakkt-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Cryptocurrency
- Digital Assets
- Trading
- Payments
- Fiat On-Ramp
- Custody
- Webhook
- FIX Protocol
---
