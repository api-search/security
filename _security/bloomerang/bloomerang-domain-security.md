---
api_specs:
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Constituents API
  slug: bloomerang-constituents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Households API
  slug: bloomerang-households-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Transactions API
  slug: bloomerang-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Interactions API
  slug: bloomerang-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Notes API
  slug: bloomerang-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Relationships API
  slug: bloomerang-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Custom Fields API
  slug: bloomerang-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Lists API
  slug: bloomerang-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Webhooks API
  slug: bloomerang-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Accounts and Users API
  slug: bloomerang-accounts-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bloomerang.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bloomerang.co
  spf: true
hosts:
- cert_expires: Aug 12 23:13:23 2026 GMT
  host: bloomerang.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: api.bloomerang.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloomerang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomerang, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bloomerang
provider_slug: bloomerang
slug: bloomerang-domain-security
source_filename: bloomerang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bloomerang.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 23:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bloomerang.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bloomerang.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bloomerang.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/security/bloomerang-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Nonprofit
- Donor Management
- CRM
- Fundraising
- Fundraising Software
---
