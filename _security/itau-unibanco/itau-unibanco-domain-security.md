---
api_specs:
- filename: itau-unibanco-accounts-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Accounts API
  slug: itau-unibanco-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-accounts-api-openapi.yml
- filename: itau-unibanco-channels-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Channels API
  slug: itau-unibanco-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-channels-api-openapi.yml
- filename: itau-unibanco-credit-cards-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Credit Cards API
  slug: itau-unibanco-credit-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-credit-cards-api-openapi.yml
- filename: itau-unibanco-discovery-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Discovery API
  slug: itau-unibanco-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-discovery-api-openapi.yml
- filename: itau-unibanco-financings-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Financings API
  slug: itau-unibanco-financings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-financings-api-openapi.yml
- filename: itau-unibanco-invoice-financings-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Invoice Financings API
  slug: itau-unibanco-invoice-financings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-invoice-financings-api-openapi.yml
- filename: itau-unibanco-loans-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Loans API
  slug: itau-unibanco-loans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-loans-api-openapi.yml
- filename: itau-unibanco-unarranged-account-overdraft-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Unarranged Account Overdraft API
  slug: itau-unibanco-unarranged-account-overdraft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-unarranged-account-overdraft-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: itau.com.br
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: itau.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Itau Unibanco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Itaú Unibanco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Itaú Unibanco
provider_slug: itau-unibanco
slug: itau-unibanco-domain-security
source_filename: itau-unibanco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: itau.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: itau.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/itau-unibanco/security/itau-unibanco-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Banking
- Financial Services
- Payments
- Pix
- Open Finance
- Brazil
- Foreign Exchange
- Credit
---
