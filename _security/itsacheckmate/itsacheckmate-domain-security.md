---
api_specs:
- filename: itsacheckmate-locations-api-openapi.yml
  format: yaml
  label: ItsaCheckmate Locations API
  slug: itsacheckmate-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsacheckmate/refs/heads/main/openapi/itsacheckmate-locations-api-openapi.yml
- filename: itsacheckmate-menus-api-openapi.yml
  format: yaml
  label: ItsaCheckmate Menus API
  slug: itsacheckmate-menus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsacheckmate/refs/heads/main/openapi/itsacheckmate-menus-api-openapi.yml
- filename: itsacheckmate-oauth-api-openapi.yml
  format: yaml
  label: ItsaCheckmate OAuth API
  slug: itsacheckmate-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsacheckmate/refs/heads/main/openapi/itsacheckmate-oauth-api-openapi.yml
- filename: itsacheckmate-orders-api-openapi.yml
  format: yaml
  label: ItsaCheckmate Orders API
  slug: itsacheckmate-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsacheckmate/refs/heads/main/openapi/itsacheckmate-orders-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: itsacheckmate.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 28 11:47:38 2026 GMT
  host: www.itsacheckmate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: openapi-itsacheckmate.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: sandbox-api.itsacheckmate.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Itsacheckmate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ItsaCheckmate, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ItsaCheckmate
provider_slug: itsacheckmate
slug: itsacheckmate-domain-security
source_filename: itsacheckmate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.itsacheckmate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:47:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: openapi-itsacheckmate.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox-api.itsacheckmate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: itsacheckmate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itsacheckmate/refs/heads/main/security/itsacheckmate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Point-of-Sale
- Online Ordering
- Delivery
- Menus
- Order
- Integration
---
