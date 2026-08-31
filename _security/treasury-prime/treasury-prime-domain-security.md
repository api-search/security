---
api_specs:
- filename: treasury-prime-accounts-api-openapi.yml
  format: yaml
  label: Treasury Prime Accounts API
  slug: treasury-prime-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-accounts-api-openapi.yml
- filename: treasury-prime-businesses-api-openapi.yml
  format: yaml
  label: Treasury Prime Businesses API
  slug: treasury-prime-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-businesses-api-openapi.yml
- filename: treasury-prime-cards-api-openapi.yml
  format: yaml
  label: Treasury Prime Cards API
  slug: treasury-prime-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-cards-api-openapi.yml
- filename: treasury-prime-health-api-openapi.yml
  format: yaml
  label: Treasury Prime Health API
  slug: treasury-prime-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-health-api-openapi.yml
- filename: treasury-prime-payments-api-openapi.yml
  format: yaml
  label: Treasury Prime Payments API
  slug: treasury-prime-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-payments-api-openapi.yml
- filename: treasury-prime-persons-api-openapi.yml
  format: yaml
  label: Treasury Prime Persons API
  slug: treasury-prime-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-persons-api-openapi.yml
- filename: treasury-prime-statements-api-openapi.yml
  format: yaml
  label: Treasury Prime Statements API
  slug: treasury-prime-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-statements-api-openapi.yml
- filename: treasury-prime-transactions-api-openapi.yml
  format: yaml
  label: Treasury Prime Transactions API
  slug: treasury-prime-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-transactions-api-openapi.yml
- filename: treasury-prime-webhooks-api-openapi.yml
  format: yaml
  label: Treasury Prime Webhooks API
  slug: treasury-prime-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: treasuryprime.com
  spf: true
hosts:
- cert_expires: Oct  9 18:07:15 2026 GMT
  host: www.treasuryprime.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developers.treasuryprime.com
  https: false
- host: sandbox.treasuryprime.com
  https: false
kind: domain-security
layout: security
method: probed
name: Treasury Prime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Treasury Prime, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Treasury Prime
provider_slug: treasury-prime
slug: treasury-prime-domain-security
source_filename: treasury-prime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.treasuryprime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 18:07:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.treasuryprime.com\n  https: false\n- host: sandbox.treasuryprime.com\n  https: false\ndomains:\n- domain: treasuryprime.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/security/treasury-prime-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- BaaS
- Banking
- Payments
- Card Issuing
- ACH
---
