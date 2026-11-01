---
api_specs:
- filename: edi-214-claim-acknowledgments-api-openapi.yml
  format: yaml
  label: Edi 214 Claim acknowledgments API
  slug: edi-214-claim-acknowledgments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-claim-acknowledgments-api-openapi.yml
- filename: edi-214-claim-submission-api-openapi.yml
  format: yaml
  label: Edi 214 Claim submission API
  slug: edi-214-claim-submission-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-claim-submission-api-openapi.yml
- filename: edi-214-coordination-of-benefits-api-openapi.yml
  format: yaml
  label: Edi 214 Coordination of benefits API
  slug: edi-214-coordination-of-benefits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-coordination-of-benefits-api-openapi.yml
- filename: edi-214-insurance-discovery-api-openapi.yml
  format: yaml
  label: Edi 214 Insurance discovery API
  slug: edi-214-insurance-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-insurance-discovery-api-openapi.yml
- filename: edi-214-payers-api-openapi.yml
  format: yaml
  label: Edi 214 Payers API
  slug: edi-214-payers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-payers-api-openapi.yml
- filename: edi-214-real-time-claim-status-api-openapi.yml
  format: yaml
  label: Edi 214 Real-time claim status API
  slug: edi-214-real-time-claim-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-real-time-claim-status-api-openapi.yml
- filename: edi-214-real-time-eligibility-check-api-openapi.yml
  format: yaml
  label: Edi 214 Real-time eligibility check API
  slug: edi-214-real-time-eligibility-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-real-time-eligibility-check-api-openapi.yml
- filename: edi-214-remittances-api-openapi.yml
  format: yaml
  label: Edi 214 Remittances API
  slug: edi-214-remittances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edi-214/openapi/edi-214-remittances-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: x12.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stedi.com
  spf: true
hosts:
- cert_expires: Oct  9 13:47:26 2026 GMT
  host: x12.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 03:39:35 2026 GMT
  host: www.stedi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.stedi.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Edi 214 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edi 214, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Edi 214
provider_slug: edi-214
slug: edi-214-domain-security
source_filename: edi-214-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: x12.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:47:26 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: www.stedi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 03:39:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stedi.com\n  https: false\ndomains:\n- domain: x12.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: stedi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/edi-214/security/edi-214-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EDI
- Logistics
- Transaction
---
