---
api_specs:
- filename: algbra-accounts-api-openapi.yml
  format: yaml
  label: Algbra Accounts API
  slug: algbra-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-accounts-api-openapi.yml
- filename: algbra-transactions-api-openapi.yml
  format: yaml
  label: Algbra Transactions API
  slug: algbra-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-transactions-api-openapi.yml
- filename: algbra-automated-payments-api-openapi.yml
  format: yaml
  label: Algbra Automated Payments API
  slug: algbra-automated-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-automated-payments-api-openapi.yml
- filename: algbra-cards-api-openapi.yml
  format: yaml
  label: Algbra Cards API
  slug: algbra-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-cards-api-openapi.yml
- filename: algbra-compliance-api-openapi.yml
  format: yaml
  label: Algbra Compliance API
  slug: algbra-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-compliance-api-openapi.yml
- filename: algbra-customers-api-openapi.yml
  format: yaml
  label: Algbra Customers API
  slug: algbra-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-customers-api-openapi.yml
- filename: algbra-investments-api-openapi.yml
  format: yaml
  label: Algbra Investments API
  slug: algbra-investments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-investments-api-openapi.yml
- filename: algbra-onboarding-prospects-business-api-openapi.yml
  format: yaml
  label: Algbra Onboarding Prospects - Business API
  slug: algbra-onboarding-prospects-business-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-onboarding-prospects-business-api-openapi.yml
- filename: algbra-onboarding-prospects-personal-api-openapi.yml
  format: yaml
  label: Algbra Onboarding Prospects - Personal API
  slug: algbra-onboarding-prospects-personal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-onboarding-prospects-personal-api-openapi.yml
- filename: algbra-partner-api-openapi.yml
  format: yaml
  label: Algbra Partner API
  slug: algbra-partner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-partner-api-openapi.yml
- filename: algbra-partners-api-openapi.yml
  format: yaml
  label: Algbra Partners API
  slug: algbra-partners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-partners-api-openapi.yml
- filename: algbra-payment-simulations-api-openapi.yml
  format: yaml
  label: Algbra Payment Simulations API
  slug: algbra-payment-simulations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-payment-simulations-api-openapi.yml
- filename: algbra-payments-api-openapi.yml
  format: yaml
  label: Algbra Payments API
  slug: algbra-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-payments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: algbra.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: algbralabs.com
  spf: true
hosts:
- cert_expires: Sep  4 03:01:59 2026 GMT
  host: www.algbra.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 09:25:25 2026 GMT
  host: developer.algbralabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: secure.tell.systems
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Algbra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Algbra, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Algbra
provider_slug: algbra
slug: algbra-domain-security
source_filename: algbra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.algbra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 03:01:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.algbralabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 09:25:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: secure.tell.systems\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: algbra.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: algbralabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/algbra/security/algbra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Fintech
- Ethical Finance
- Banking as a Service
---
