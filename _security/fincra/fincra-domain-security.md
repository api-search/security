---
api_specs:
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Collections API
  slug: fincra-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Payouts / Disbursements API
  slug: fincra-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Conversions / FX API
  slug: fincra-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Quotes API
  slug: fincra-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Beneficiaries API
  slug: fincra-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Virtual Accounts API
  slug: fincra-virtual-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Banks & Account Resolution API
  slug: fincra-banks-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Webhooks
  slug: fincra-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fincra.com
  spf: true
hosts:
- cert_expires: Aug 20 07:20:57 2026 GMT
  host: www.fincra.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 15:02:25 2026 GMT
  host: docs.fincra.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 07:20:57 2026 GMT
  host: api.fincra.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fincra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fincra, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fincra
provider_slug: fincra
slug: fincra-domain-security
source_filename: fincra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fincra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 07:20:57 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.fincra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:02:25 2026 GMT\n  hsts: null\n- host: api.fincra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 07:20:57 2026 GMT\n  hsts: null\ndomains:\n- domain: fincra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/security/fincra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Cross-Border
- Collections
- Payouts
- FX
- Fintech
- Africa
---
