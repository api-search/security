---
api_specs:
- filename: criteo-retail-media-api-openapi.yml
  format: yaml
  label: Criteo Retail Media API
  slug: criteo-retail-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-retail-media-api-openapi.yml
- filename: criteo-marketing-solutions-api-openapi.yml
  format: yaml
  label: Criteo Marketing Solutions API
  slug: criteo-marketing-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-marketing-solutions-api-openapi.yml
- filename: criteo-commerce-grid-api-openapi.yml
  format: yaml
  label: Criteo Commerce Grid API
  slug: criteo-commerce-grid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-commerce-grid-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
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
- cert_expires: Oct 29 23:59:59 2026 GMT
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
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.criteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:49:57 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developers.criteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:16:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.criteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: criteo.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/security/criteo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Agent Skills
- Analytics
- Audiences
- Campaigns
- Catalog
- Commerce
- Commerce Media
- Display Advertising
- Marketing
- MCP
- Media
- OAuth 2.0
- OpenAPI
- Reporting
- Retail
- Retail Media
- Sponsored Products
---
