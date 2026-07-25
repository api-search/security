---
api_specs:
- filename: marketman-accounts-api-openapi.yml
  format: yaml
  label: MarketMan Accounts API
  slug: marketman-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-accounts-api-openapi.yml
- filename: marketman-authentication-api-openapi.yml
  format: yaml
  label: MarketMan Authentication API
  slug: marketman-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-authentication-api-openapi.yml
- filename: marketman-deliveries-api-openapi.yml
  format: yaml
  label: MarketMan Deliveries API
  slug: marketman-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-deliveries-api-openapi.yml
- filename: marketman-docs-api-openapi.yml
  format: yaml
  label: MarketMan Docs API
  slug: marketman-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-docs-api-openapi.yml
- filename: marketman-inventory-api-openapi.yml
  format: yaml
  label: MarketMan Inventory API
  slug: marketman-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-inventory-api-openapi.yml
- filename: marketman-items-api-openapi.yml
  format: yaml
  label: MarketMan Items API
  slug: marketman-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-items-api-openapi.yml
- filename: marketman-orders-api-openapi.yml
  format: yaml
  label: MarketMan Orders API
  slug: marketman-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-orders-api-openapi.yml
- filename: marketman-recipes-api-openapi.yml
  format: yaml
  label: MarketMan Recipes API
  slug: marketman-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-recipes-api-openapi.yml
- filename: marketman-webhooks-api-openapi.yml
  format: yaml
  label: MarketMan Webhooks API
  slug: marketman-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marketman.com
  spf: true
hosts:
- cert_expires: Aug 12 09:42:19 2026 GMT
  host: www.marketman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 12:02:21 2026 GMT
  host: api-doc.marketman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 12:02:21 2026 GMT
  host: api.marketman.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marketman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarketMan, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MarketMan
provider_slug: marketman
slug: marketman-domain-security
source_filename: marketman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marketman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 09:42:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-doc.marketman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:02:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.marketman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:02:21 2026 GMT\n  hsts: false\ndomains:\n- domain: marketman.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/security/marketman-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Inventory
- Purchasing
- Supply Chain
- Food Service
---
