---
api_specs:
- filename: alloy-bank-accounts-api-openapi.yml
  format: yaml
  label: Alloy Bank Accounts API
  slug: alloy-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-bank-accounts-api-openapi.yml
- filename: alloy-documents-api-openapi.yml
  format: yaml
  label: Alloy Documents API
  slug: alloy-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-documents-api-openapi.yml
- filename: alloy-entities-api-openapi.yml
  format: yaml
  label: Alloy Entities API
  slug: alloy-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-entities-api-openapi.yml
- filename: alloy-entity-groups-api-openapi.yml
  format: yaml
  label: Alloy Entity Groups API
  slug: alloy-entity-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-entity-groups-api-openapi.yml
- filename: alloy-evaluations-api-openapi.yml
  format: yaml
  label: Alloy Evaluations API
  slug: alloy-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-evaluations-api-openapi.yml
- filename: alloy-events-api-openapi.yml
  format: yaml
  label: Alloy Events API
  slug: alloy-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-events-api-openapi.yml
- filename: alloy-investigations-api-openapi.yml
  format: yaml
  label: Alloy Investigations API
  slug: alloy-investigations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-investigations-api-openapi.yml
- filename: alloy-journeys-api-openapi.yml
  format: yaml
  label: Alloy Journeys API
  slug: alloy-journeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-journeys-api-openapi.yml
- filename: alloy-oauth-api-openapi.yml
  format: yaml
  label: Alloy OAuth API
  slug: alloy-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-oauth-api-openapi.yml
- filename: alloy-transactions-api-openapi.yml
  format: yaml
  label: Alloy Transactions API
  slug: alloy-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alloy.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alloy.co
  spf: true
hosts:
- cert_expires: Aug 24 11:19:46 2026 GMT
  host: www.alloy.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 21:53:47 2026 GMT
  host: developer.alloy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: sandbox.alloy.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alloy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alloy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Alloy
provider_slug: alloy
slug: alloy-domain-security
source_filename: alloy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alloy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 11:19:46 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.alloy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 21:53:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.alloy.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: alloy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: alloy.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/security/alloy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Identity Verification
- KYC
- KYB
- Fraud Prevention
- Compliance
- Onboarding
- Transaction Monitoring
- Risk Decisioning
- AML
- Fintech
---
