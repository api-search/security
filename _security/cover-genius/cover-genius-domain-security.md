---
api_specs:
- filename: cover-genius-openapi.yml
  format: yaml
  label: XCover Offers API
  slug: xcover-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cover-genius/refs/heads/main/openapi/cover-genius-openapi.yml
- filename: cover-genius-openapi.yml
  format: yaml
  label: XCover Bookings and Policies API
  slug: xcover-bookings-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cover-genius/refs/heads/main/openapi/cover-genius-openapi.yml
- filename: cover-genius-openapi.yml
  format: yaml
  label: XClaim Claims API
  slug: xclaim-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cover-genius/refs/heads/main/openapi/cover-genius-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: covergenius.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xcover.com
  spf: true
hosts:
- cert_expires: Oct  8 20:00:46 2026 GMT
  host: www.covergenius.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 15:12:01 2026 GMT
  host: partner-docs.covergenius.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 21:44:43 2026 GMT
  host: api.xcover.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cover Genius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cover Genius, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cover Genius
provider_slug: cover-genius
slug: cover-genius-domain-security
source_filename: cover-genius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.covergenius.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 20:00:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: partner-docs.covergenius.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:12:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.xcover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:44:43 2026 GMT\n  hsts: null\ndomains:\n- domain: covergenius.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: xcover.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cover-genius/refs/heads/main/security/cover-genius-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- Embedded Insurance
- Protection
- Claims
---
