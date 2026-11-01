---
api_specs:
- filename: scento-contrast-api-openapi.yml
  format: yaml
  label: Scento Compendium API Contrast API
  slug: scento-contrast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scento/openapi/scento-contrast-api-openapi.yml
- filename: scento-perfume-portrait-api-openapi.yml
  format: yaml
  label: Scento Compendium API Perfume portrait API
  slug: scento-perfume-portrait-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scento/openapi/scento-perfume-portrait-api-openapi.yml
- filename: scento-scent-neighbours-api-openapi.yml
  format: yaml
  label: Scento Compendium API Scent neighbours API
  slug: scento-scent-neighbours-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scento/openapi/scento-scent-neighbours-api-openapi.yml
- filename: scento-search-the-compendium-api-openapi.yml
  format: yaml
  label: Scento Compendium API Search the Compendium API
  slug: scento-search-the-compendium-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scento/openapi/scento-search-the-compendium-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scento.com
  spf: true
hosts:
- cert_expires: Nov 23 02:37:36 2026 GMT
  host: www.scento.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Scento Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scento Compendium API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scento Compendium API
provider_slug: scento
slug: scento-domain-security
source_filename: scento-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scento.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 02:37:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scento.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/scento/security/scento-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-commerce
- Fragrance
- Decant
- API
---
