---
api_specs:
- filename: short-io-audit-api-openapi.yml
  format: yaml
  label: Short.io Audit API
  slug: short-io-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-audit-api-openapi.yml
- filename: short-io-domain-dns-api-openapi.yml
  format: yaml
  label: Short.io Domain DNS API
  slug: short-io-domain-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-domain-dns-api-openapi.yml
- filename: short-io-domains-api-openapi.yml
  format: yaml
  label: Short.io Domains API
  slug: short-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-domains-api-openapi.yml
- filename: short-io-link-bundles-api-openapi.yml
  format: yaml
  label: Short.io Link Bundles API
  slug: short-io-link-bundles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-link-bundles-api-openapi.yml
- filename: short-io-link-duplication-api-openapi.yml
  format: yaml
  label: Short.io Link Duplication API
  slug: short-io-link-duplication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-link-duplication-api-openapi.yml
- filename: short-io-link-management-api-openapi.yml
  format: yaml
  label: Short.io Link Management API
  slug: short-io-link-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-link-management-api-openapi.yml
- filename: short-io-link-queries-api-openapi.yml
  format: yaml
  label: Short.io Link queries API
  slug: short-io-link-queries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-link-queries-api-openapi.yml
- filename: short-io-link-targeting-api-openapi.yml
  format: yaml
  label: Short.io Link Targeting API
  slug: short-io-link-targeting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-link-targeting-api-openapi.yml
- filename: short-io-organizations-api-openapi.yml
  format: yaml
  label: Short.io Organizations API
  slug: short-io-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-organizations-api-openapi.yml
- filename: short-io-posts-api-openapi.yml
  format: yaml
  label: Short.io Posts API
  slug: short-io-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-posts-api-openapi.yml
- filename: short-io-qr-codes-api-openapi.yml
  format: yaml
  label: Short.io QR Codes API
  slug: short-io-qr-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-qr-codes-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: short.io
  spf: true
hosts:
- cert_expires: Nov 28 09:58:12 2026 GMT
  host: short.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Short Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Short.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Short.io
provider_slug: short-io
slug: short-io-domain-security
source_filename: short-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: short.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 09:58:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: short.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/short-io/security/short-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- URL-shortening
- Analytics
- QR-codes
- Enterprise
- Integrations
---
