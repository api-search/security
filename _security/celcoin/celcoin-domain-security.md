---
api_specs:
- filename: celcoin-annotationcompetencecalendar-api-openapi.yml
  format: yaml
  label: Celcoin AnnotationCompetenceCalendar API
  slug: celcoin-annotationcompetencecalendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-annotationcompetencecalendar-api-openapi.yml
- filename: celcoin-bankcorrespondentagent-api-openapi.yml
  format: yaml
  label: Celcoin BankCorrespondentAgent API
  slug: celcoin-bankcorrespondentagent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-bankcorrespondentagent-api-openapi.yml
- filename: celcoin-consignee-api-openapi.yml
  format: yaml
  label: Celcoin Consignee API
  slug: celcoin-consignee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-consignee-api-openapi.yml
- filename: celcoin-files-api-openapi.yml
  format: yaml
  label: Celcoin Files API
  slug: celcoin-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-files-api-openapi.yml
- filename: celcoin-guarantee-api-openapi.yml
  format: yaml
  label: Celcoin Guarantee API
  slug: celcoin-guarantee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-guarantee-api-openapi.yml
- filename: celcoin-legacyguarantee-api-openapi.yml
  format: yaml
  label: Celcoin LegacyGuarantee API
  slug: celcoin-legacyguarantee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-legacyguarantee-api-openapi.yml
- filename: celcoin-legalperson-api-openapi.yml
  format: yaml
  label: Celcoin LegalPerson API
  slug: celcoin-legalperson-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-legalperson-api-openapi.yml
- filename: celcoin-naturalperson-api-openapi.yml
  format: yaml
  label: Celcoin NaturalPerson API
  slug: celcoin-naturalperson-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-naturalperson-api-openapi.yml
- filename: celcoin-outstandingbalance-api-openapi.yml
  format: yaml
  label: Celcoin OutstandingBalance API
  slug: celcoin-outstandingbalance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-outstandingbalance-api-openapi.yml
- filename: celcoin-proposal-api-openapi.yml
  format: yaml
  label: Celcoin Proposal API
  slug: celcoin-proposal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-proposal-api-openapi.yml
- filename: celcoin-settlement-api-openapi.yml
  format: yaml
  label: Celcoin Settlement API
  slug: celcoin-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-settlement-api-openapi.yml
- filename: celcoin-taggingjourney-api-openapi.yml
  format: yaml
  label: Celcoin TaggingJourney API
  slug: celcoin-taggingjourney-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-taggingjourney-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: celcoin.com.br
  spf: true
hosts:
- cert_expires: Oct  8 15:00:37 2026 GMT
  host: www.celcoin.com.br
  hsts: true
  hsts_max_age: 10368000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 03:38:52 2026 GMT
  host: developers.celcoin.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:12:30 2026 GMT
  host: api.openfinance.celcoin.com.br
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Celcoin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celcoin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Celcoin
provider_slug: celcoin
slug: celcoin-domain-security
source_filename: celcoin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.celcoin.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 15:00:37 2026 GMT\n  hsts: true\n  hsts_max_age: 10368000\n- host: developers.celcoin.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 03:38:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openfinance.celcoin.com.br\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 23:12:30 2026 GMT\n  hsts: null\ndomains:\n- domain: celcoin.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/security/celcoin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking as a Service
- Backend-as-a-Service
- Pix
- Boleto
- TED
- Bill Payments
- Prepaid Cards
- Digital Accounts
- Open Banking
- Open Finance
- Credit
- Fintech
- Brazil
- Financial Infrastructure
---
