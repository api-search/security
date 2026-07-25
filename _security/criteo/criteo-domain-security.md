---
api_specs:
- filename: criteo-accounts-api-openapi.yml
  format: yaml
  label: Criteo Accounts API
  slug: criteo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-accounts-api-openapi.yml
- filename: criteo-audiences-api-openapi.yml
  format: yaml
  label: Criteo Audiences API
  slug: criteo-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-audiences-api-openapi.yml
- filename: criteo-authentication-api-openapi.yml
  format: yaml
  label: Criteo Authentication API
  slug: criteo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-authentication-api-openapi.yml
- filename: criteo-balances-api-openapi.yml
  format: yaml
  label: Criteo Balances API
  slug: criteo-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-balances-api-openapi.yml
- filename: criteo-campaigns-api-openapi.yml
  format: yaml
  label: Criteo Campaigns API
  slug: criteo-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-campaigns-api-openapi.yml
- filename: criteo-catalogs-api-openapi.yml
  format: yaml
  label: Criteo Catalogs API
  slug: criteo-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-catalogs-api-openapi.yml
- filename: criteo-categories-api-openapi.yml
  format: yaml
  label: Criteo Categories API
  slug: criteo-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-categories-api-openapi.yml
- filename: criteo-keywords-api-openapi.yml
  format: yaml
  label: Criteo Keywords API
  slug: criteo-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-keywords-api-openapi.yml
- filename: criteo-lineitems-api-openapi.yml
  format: yaml
  label: Criteo LineItems API
  slug: criteo-lineitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-lineitems-api-openapi.yml
- filename: criteo-products-api-openapi.yml
  format: yaml
  label: Criteo Products API
  slug: criteo-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-products-api-openapi.yml
- filename: criteo-reports-api-openapi.yml
  format: yaml
  label: Criteo Reports API
  slug: criteo-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-reports-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: criteo.com
  spf: true
hosts:
- cert_expires: Sep 14 13:49:57 2026 GMT
  host: www.criteo.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 13:16:40 2026 GMT
  host: developers.criteo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 23:59:59 2026 GMT
  host: api.criteo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Criteo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Criteo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Criteo
provider_slug: criteo
slug: criteo-domain-security
source_filename: criteo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.criteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:49:57 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developers.criteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:16:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.criteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: criteo.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/security/criteo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Audiences
- Campaigns
- Catalog
- Commerce
- Display Advertising
- Marketing
- Media
- OAuth 2.0
- Reporting
- Retail
- Retail Media
---
