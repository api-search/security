---
api_specs:
- filename: gnosis-pay-auth-api-openapi.yml
  format: yaml
  label: Gnosis Pay Auth API
  slug: gnosis-pay-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-auth-api-openapi.yml
- filename: gnosis-pay-cards-api-openapi.yml
  format: yaml
  label: Gnosis Pay Cards API
  slug: gnosis-pay-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-cards-api-openapi.yml
- filename: gnosis-pay-health-api-openapi.yml
  format: yaml
  label: Gnosis Pay Health API
  slug: gnosis-pay-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-health-api-openapi.yml
- filename: gnosis-pay-kyc-api-openapi.yml
  format: yaml
  label: Gnosis Pay KYC API
  slug: gnosis-pay-kyc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-kyc-api-openapi.yml
- filename: gnosis-pay-pci-api-openapi.yml
  format: yaml
  label: Gnosis Pay PCI API
  slug: gnosis-pay-pci-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-pci-api-openapi.yml
- filename: gnosis-pay-phone-api-openapi.yml
  format: yaml
  label: Gnosis Pay Phone API
  slug: gnosis-pay-phone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-phone-api-openapi.yml
- filename: gnosis-pay-source-of-funds-api-openapi.yml
  format: yaml
  label: Gnosis Pay Source of Funds API
  slug: gnosis-pay-source-of-funds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-source-of-funds-api-openapi.yml
- filename: gnosis-pay-terms-api-openapi.yml
  format: yaml
  label: Gnosis Pay Terms API
  slug: gnosis-pay-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-terms-api-openapi.yml
- filename: gnosis-pay-user-account-api-openapi.yml
  format: yaml
  label: Gnosis Pay User Account API
  slug: gnosis-pay-user-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-user-account-api-openapi.yml
- filename: gnosis-pay-user-api-openapi.yml
  format: yaml
  label: Gnosis Pay User API
  slug: gnosis-pay-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-user-api-openapi.yml
- filename: gnosis-pay-user-movements-api-openapi.yml
  format: yaml
  label: Gnosis Pay User Movements API
  slug: gnosis-pay-user-movements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-user-movements-api-openapi.yml
- filename: gnosis-pay-3-ds-api-openapi.yml
  format: yaml
  label: Gnosis Pay 3 DS API
  slug: gnosis-pay-3-ds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-3-ds-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:devops@gnosis.io"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gnosispay.com
  spf: true
hosts:
- cert_expires: Jan  8 13:47:48 2027 GMT
  host: gnosispay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gnosis Pay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gnosis Pay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Gnosis Pay
provider_slug: gnosis-pay
slug: gnosis-pay-domain-security
source_filename: gnosis-pay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gnosispay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 13:47:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gnosispay.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:devops@gnosis.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gnosis-pay/security/gnosis-pay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- Crypto
- Stablecoin
- API
---
