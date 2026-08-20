---
api_specs:
- filename: kintsugi-address-validation-api-openapi.yml
  format: yaml
  label: Kintsugi Address Validation API
  slug: kintsugi-address-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-address-validation-api-openapi.yml
- filename: kintsugi-customers-api-openapi.yml
  format: yaml
  label: Kintsugi Customers API
  slug: kintsugi-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-customers-api-openapi.yml
- filename: kintsugi-exemptions-api-openapi.yml
  format: yaml
  label: Kintsugi Exemptions API
  slug: kintsugi-exemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-exemptions-api-openapi.yml
- filename: kintsugi-filings-api-openapi.yml
  format: yaml
  label: Kintsugi Filings API
  slug: kintsugi-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-filings-api-openapi.yml
- filename: kintsugi-nexus-api-openapi.yml
  format: yaml
  label: Kintsugi Nexus API
  slug: kintsugi-nexus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-nexus-api-openapi.yml
- filename: kintsugi-products-api-openapi.yml
  format: yaml
  label: Kintsugi Products API
  slug: kintsugi-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-products-api-openapi.yml
- filename: kintsugi-registrations-api-openapi.yml
  format: yaml
  label: Kintsugi Registrations API
  slug: kintsugi-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-registrations-api-openapi.yml
- filename: kintsugi-tax-estimation-api-openapi.yml
  format: yaml
  label: Kintsugi Tax Estimation API
  slug: kintsugi-tax-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-tax-estimation-api-openapi.yml
- filename: kintsugi-transactions-api-openapi.yml
  format: yaml
  label: Kintsugi Transactions API
  slug: kintsugi-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/openapi/kintsugi-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trykintsugi.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.trykintsugi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 02:39:17 2026 GMT
  host: docs.trykintsugi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: api.trykintsugi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kintsugi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kintsugi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kintsugi
provider_slug: kintsugi
slug: kintsugi-domain-security
source_filename: kintsugi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trykintsugi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\n- host: docs.trykintsugi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 02:39:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.trykintsugi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: trykintsugi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/security/kintsugi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Tax
- Tax Compliance
- Tax Automation
- VAT
- GST
- Nexus
- Artificial Intelligence
---
