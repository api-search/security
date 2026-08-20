---
api_specs:
- filename: givebutter-campaigns-api-openapi.yml
  format: yaml
  label: Givebutter Campaigns API
  slug: givebutter-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-campaigns-api-openapi.yml
- filename: givebutter-contacts-api-openapi.yml
  format: yaml
  label: Givebutter Contacts API
  slug: givebutter-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-contacts-api-openapi.yml
- filename: givebutter-discount-codes-api-openapi.yml
  format: yaml
  label: Givebutter Discount Codes API
  slug: givebutter-discount-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-discount-codes-api-openapi.yml
- filename: givebutter-funds-api-openapi.yml
  format: yaml
  label: Givebutter Funds API
  slug: givebutter-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-funds-api-openapi.yml
- filename: givebutter-payouts-api-openapi.yml
  format: yaml
  label: Givebutter Payouts API
  slug: givebutter-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-payouts-api-openapi.yml
- filename: givebutter-plans-api-openapi.yml
  format: yaml
  label: Givebutter Plans API
  slug: givebutter-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-plans-api-openapi.yml
- filename: givebutter-tickets-api-openapi.yml
  format: yaml
  label: Givebutter Tickets API
  slug: givebutter-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-tickets-api-openapi.yml
- filename: givebutter-transactions-api-openapi.yml
  format: yaml
  label: Givebutter Transactions API
  slug: givebutter-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-transactions-api-openapi.yml
- filename: givebutter-webhooks-api-openapi.yml
  format: yaml
  label: Givebutter Webhooks API
  slug: givebutter-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/openapi/givebutter-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: givebutter.com
  spf: true
hosts:
- cert_expires: Aug 14 02:43:35 2026 GMT
  host: givebutter.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 01:21:05 2026 GMT
  host: docs.givebutter.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 07:53:47 2026 GMT
  host: api.givebutter.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Givebutter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Givebutter, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Givebutter
provider_slug: givebutter
slug: givebutter-domain-security
source_filename: givebutter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: givebutter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 02:43:35 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.givebutter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 01:21:05 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.givebutter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:53:47 2026 GMT\n  hsts: null\ndomains:\n- domain: givebutter.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/givebutter/refs/heads/main/security/givebutter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Donations
- Fundraising
- Non-Profit
---
