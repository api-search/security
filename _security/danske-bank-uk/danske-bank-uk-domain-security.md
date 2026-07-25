---
api_specs:
- filename: danske-bank-uk-opendata-openapi.json
  format: json
  label: Danske Bank (UK) Open Data API
  slug: danske-bank-uk-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-opendata-openapi.json
- filename: danske-bank-uk-account-transaction-openapi.json
  format: json
  label: Danske Bank (UK) Account and Transaction API
  slug: danske-bank-uk-account-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-account-transaction-openapi.json
- filename: danske-bank-uk-payment-initiation-openapi.json
  format: json
  label: Danske Bank (UK) Payment Initiation API
  slug: danske-bank-uk-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-payment-initiation-openapi.json
- filename: danske-bank-uk-confirmation-of-funds-openapi.json
  format: json
  label: Danske Bank (UK) Confirmation of Funds API
  slug: danske-bank-uk-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-confirmation-of-funds-openapi.json
- filename: danske-bank-uk-variable-recurring-payments-openapi.json
  format: json
  label: Danske Bank (UK) Variable Recurring Payments API
  slug: danske-bank-uk-variable-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-variable-recurring-payments-openapi.json
- filename: danske-bank-uk-events-openapi.json
  format: json
  label: Danske Bank (UK) Events API
  slug: danske-bank-uk-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-events-openapi.json
- filename: danske-bank-uk-account-transaction-balance-premium-openapi.json
  format: json
  label: Danske Bank (UK) Account Transaction & Balance API
  slug: danske-bank-uk-account-transaction-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-account-transaction-balance-premium-openapi.json
- filename: danske-bank-uk-payment-collection-premium-openapi.json
  format: json
  label: Danske Bank (UK) Payment Collection API
  slug: danske-bank-uk-payment-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-payment-collection-premium-openapi.json
- filename: danske-bank-uk-premium-payment-initiation-openapi.json
  format: json
  label: Danske Bank (UK) Premium Payment Initiation API
  slug: danske-bank-uk-premium-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-premium-payment-initiation-openapi.json
- filename: danske-bank-uk-fx-trade-report-openapi.json
  format: json
  label: Danske Bank (UK) FX Trade Report API
  slug: danske-bank-uk-fx-trade-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-fx-trade-report-openapi.json
- filename: danske-bank-uk-fx-trade-execution-openapi.json
  format: json
  label: Danske Bank (UK) FX Trade Execution API
  slug: danske-bank-uk-fx-trade-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-fx-trade-execution-openapi.json
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issuewild ";"
  - 0 iodef "mailto:security.administration@danskebank.dk"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: danskebank.co.uk
  spf: true
- caa:
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  - 0 iodef "mailto:security.administration@danskebank.dk"
  - 0 issue "amazon.com"
  - 0 issue "buypass.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: danskebank.com
  spf: true
hosts:
- cert_expires: Mar 28 17:37:18 2027 GMT
  host: www.danskebank.co.uk
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 05:51:28 2027 GMT
  host: developers.danskebank.com
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 03:17:26 2026 GMT
  host: obp-data.danskebank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Danske Bank Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Danske Bank (UK), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Danske Bank (UK)
provider_slug: danske-bank-uk
slug: danske-bank-uk-domain-security
source_filename: danske-bank-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.danskebank.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 28 17:37:18 2027 GMT\n  hsts: true\n  hsts_max_age: 157680000\n- host: developers.danskebank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 05:51:28 2027 GMT\n  hsts: true\n  hsts_max_age: 157680000\n- host: obp-data.danskebank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:17:26 2026 GMT\n  hsts: null\ndomains:\n- domain: danskebank.co.uk\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:security.administration@danskebank.dk\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: danskebank.com\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 iodef \"mailto:security.administration@danskebank.dk\"\n\
  \  - 0 issue \"amazon.com\"\n  - 0 issue \"buypass.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/security/danske-bank-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Northern Ireland
- Payments
- Account Information
- FAPI
- Fintech
---
