---
api_specs:
- filename: doordash-addresses-api-openapi.yml
  format: yaml
  label: doordash Addresses API
  slug: doordash-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-addresses-api-openapi.yml
- filename: doordash-businesses-api-openapi.yml
  format: yaml
  label: doordash Businesses API
  slug: doordash-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-businesses-api-openapi.yml
- filename: doordash-catalog-api-openapi.yml
  format: yaml
  label: doordash Catalog API
  slug: doordash-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-catalog-api-openapi.yml
- filename: doordash-deliveries-api-openapi.yml
  format: yaml
  label: doordash Deliveries API
  slug: doordash-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-deliveries-api-openapi.yml
- filename: doordash-inventory-api-openapi.yml
  format: yaml
  label: doordash Inventory API
  slug: doordash-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-inventory-api-openapi.yml
- filename: doordash-items-api-openapi.yml
  format: yaml
  label: doordash Items API
  slug: doordash-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-items-api-openapi.yml
- filename: doordash-menus-api-openapi.yml
  format: yaml
  label: doordash Menus API
  slug: doordash-menus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-menus-api-openapi.yml
- filename: doordash-orders-api-openapi.yml
  format: yaml
  label: doordash Orders API
  slug: doordash-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-orders-api-openapi.yml
- filename: doordash-promotions-api-openapi.yml
  format: yaml
  label: doordash Promotions API
  slug: doordash-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-promotions-api-openapi.yml
- filename: doordash-quotes-api-openapi.yml
  format: yaml
  label: doordash Quotes API
  slug: doordash-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-quotes-api-openapi.yml
- filename: doordash-reports-api-openapi.yml
  format: yaml
  label: doordash Reports API
  slug: doordash-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-reports-api-openapi.yml
- filename: doordash-stores-api-openapi.yml
  format: yaml
  label: doordash Stores API
  slug: doordash-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-stores-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:caa-reports@doordash.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: doordash.com
  spf: true
hosts:
- cert_expires: Sep  8 03:29:44 2026 GMT
  host: www.doordash.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:44:30 2026 GMT
  host: developer.doordash.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:44:30 2026 GMT
  host: openapi.doordash.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doordash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doordash, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Doordash
provider_slug: doordash
slug: doordash-domain-security
source_filename: doordash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doordash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 03:29:44 2026 GMT\n  hsts: null\n- host: developer.doordash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:44:30 2026 GMT\n  hsts: null\n- host: openapi.doordash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:44:30 2026 GMT\n  hsts: null\ndomains:\n- domain: doordash.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:caa-reports@doordash.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/security/doordash-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags: []
---
