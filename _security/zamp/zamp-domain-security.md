---
api_specs:
- filename: zamp-openapi-generated.yml
  format: yaml
  label: Zamp API
  slug: zamp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/_ae-authored/zamp-openapi-generated.yml
- filename: zamp-addresses-api-openapi.yml
  format: yaml
  label: Zamp Addresses API
  slug: zamp-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/zamp-addresses-api-openapi.yml
- filename: zamp-calculations-api-openapi.yml
  format: yaml
  label: Zamp Calculations API
  slug: zamp-calculations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/zamp-calculations-api-openapi.yml
- filename: zamp-companies-api-openapi.yml
  format: yaml
  label: Zamp Companies API
  slug: zamp-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/zamp-companies-api-openapi.yml
- filename: zamp-filings-api-openapi.yml
  format: yaml
  label: Zamp Filings API
  slug: zamp-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/zamp-filings-api-openapi.yml
- filename: zamp-registrations-api-openapi.yml
  format: yaml
  label: Zamp Registrations API
  slug: zamp-registrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/zamp-registrations-api-openapi.yml
- filename: zamp-tax-codes-api-openapi.yml
  format: yaml
  label: Zamp Tax Codes API
  slug: zamp-tax-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/zamp-tax-codes-api-openapi.yml
- filename: zamp-transactions-api-openapi.yml
  format: yaml
  label: Zamp Transactions API
  slug: zamp-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zamp/openapi/zamp-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zamp.com
  spf: true
hosts:
- cert_expires: Jan  3 22:25:54 2027 GMT
  host: zamp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zamp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zamp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zamp
provider_slug: zamp
slug: zamp-domain-security
source_filename: zamp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 22:25:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zamp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/zamp/security/zamp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sales Tax
- Automation
- Compliance
---
