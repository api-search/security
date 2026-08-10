---
api_specs:
- filename: scryfall-bulk-data-api-openapi.yml
  format: yaml
  label: Scryfall Bulk Data API
  slug: scryfall-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scryfall/refs/heads/main/openapi/scryfall-bulk-data-api-openapi.yml
- filename: scryfall-cards-api-openapi.yml
  format: yaml
  label: Scryfall Cards API
  slug: scryfall-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scryfall/refs/heads/main/openapi/scryfall-cards-api-openapi.yml
- filename: scryfall-catalogs-api-openapi.yml
  format: yaml
  label: Scryfall Catalogs API
  slug: scryfall-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scryfall/refs/heads/main/openapi/scryfall-catalogs-api-openapi.yml
- filename: scryfall-migrations-api-openapi.yml
  format: yaml
  label: Scryfall Migrations API
  slug: scryfall-migrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scryfall/refs/heads/main/openapi/scryfall-migrations-api-openapi.yml
- filename: scryfall-rulings-api-openapi.yml
  format: yaml
  label: Scryfall Rulings API
  slug: scryfall-rulings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scryfall/refs/heads/main/openapi/scryfall-rulings-api-openapi.yml
- filename: scryfall-sets-api-openapi.yml
  format: yaml
  label: Scryfall Sets API
  slug: scryfall-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scryfall/refs/heads/main/openapi/scryfall-sets-api-openapi.yml
- filename: scryfall-symbology-api-openapi.yml
  format: yaml
  label: Scryfall Symbology API
  slug: scryfall-symbology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scryfall/refs/heads/main/openapi/scryfall-symbology-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scryfall.com
  spf: true
hosts:
- cert_expires: Oct  3 02:03:00 2026 GMT
  host: scryfall.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 02:03:00 2026 GMT
  host: api.scryfall.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scryfall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scryfall, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Scryfall
provider_slug: scryfall
slug: scryfall-domain-security
source_filename: scryfall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scryfall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:03:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.scryfall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:03:00 2026 GMT\n  hsts: null\ndomains:\n- domain: scryfall.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scryfall/refs/heads/main/security/scryfall-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Games And Comics
- Magic The Gathering
- Card Data
- Open Data
- Free
- Community Funded
- Public APIs
---
