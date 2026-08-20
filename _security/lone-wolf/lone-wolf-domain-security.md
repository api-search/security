---
api_specs:
- filename: lone-wolf-transact-api-openapi.yml
  format: yaml
  label: Lone Wolf Transact API
  slug: lone-wolf-transact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-transact-api-openapi.yml
- filename: lone-wolf-deals-api-openapi.yml
  format: yaml
  label: Lone Wolf Deals API
  slug: lone-wolf-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-deals-api-openapi.yml
- filename: lone-wolf-back-office-online-api-openapi.yml
  format: yaml
  label: Lone Wolf Back Office API
  slug: lone-wolf-back-office-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-back-office-online-api-openapi.yml
- filename: lone-wolf-authentisign-api-openapi.yml
  format: yaml
  label: Lone Wolf Authentisign API
  slug: lone-wolf-authentisign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-authentisign-api-openapi.yml
- filename: lone-wolf-transactiondesk-api-openapi.yml
  format: yaml
  label: Lone Wolf TransactionDesk Partner API
  slug: lone-wolf-transactiondesk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-transactiondesk-api-openapi.yml
- filename: lone-wolf-zipform-api-openapi.yml
  format: yaml
  label: Lone Wolf zipForm Partner API
  slug: lone-wolf-zipform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-zipform-api-openapi.yml
- filename: lone-wolf-wolfconnect-api-openapi.yml
  format: yaml
  label: Lone Wolf WolfConnect API
  slug: lone-wolf-wolfconnect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-wolfconnect-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lwolf.com
  spf: true
hosts:
- cert_expires: Sep 27 06:25:57 2026 GMT
  host: www.lwolf.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 06:14:18 2026 GMT
  host: apidocs.lwolf.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 22:38:08 2026 GMT
  host: gateway.lwolf.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lone Wolf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lone Wolf Technologies, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lone Wolf Technologies
provider_slug: lone-wolf
slug: lone-wolf-domain-security
source_filename: lone-wolf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lwolf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:25:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apidocs.lwolf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 06:14:18 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: gateway.lwolf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:38:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lwolf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/security/lone-wolf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- United States
- PropTech
- Transaction
- Transaction Management
- Brokerage Back Office
- Real Estate Accounting
- Commissions
- Forms
- zipForm
- TransactionDesk
- E-Signature
- CMA
- Valuation
- CRM
- MLS
- Real Estate Agents
- Brokers
---
