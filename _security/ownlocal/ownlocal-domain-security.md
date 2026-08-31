---
api_specs:
- filename: ownlocal-ads-api-openapi.yml
  format: yaml
  label: OwnLocal Ads API
  slug: ownlocal-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownlocal/refs/heads/main/openapi/ownlocal-ads-api-openapi.yml
- filename: ownlocal-businesses-api-openapi.yml
  format: yaml
  label: OwnLocal Businesses API
  slug: ownlocal-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownlocal/refs/heads/main/openapi/ownlocal-businesses-api-openapi.yml
- filename: ownlocal-categories-api-openapi.yml
  format: yaml
  label: OwnLocal Categories API
  slug: ownlocal-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownlocal/refs/heads/main/openapi/ownlocal-categories-api-openapi.yml
- filename: ownlocal-reports-data-api-api-openapi.yml
  format: yaml
  label: OwnLocal Reports Data API
  slug: ownlocal-reports-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownlocal/refs/heads/main/openapi/ownlocal-reports-data-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ownlocal.com
  spf: true
hosts:
- cert_expires: Nov 10 18:26:48 2026 GMT
  host: ownlocal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 11:55:50 2026 GMT
  host: api.docs.ownlocal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 01:07:12 2026 GMT
  host: admin.austin.ownlocal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ownlocal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OwnLocal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OwnLocal
provider_slug: ownlocal
slug: ownlocal-domain-security
source_filename: ownlocal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ownlocal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 18:26:48 2026 GMT\n  hsts: false\n- host: api.docs.ownlocal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 11:55:50 2026 GMT\n  hsts: false\n- host: admin.austin.ownlocal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 01:07:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ownlocal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ownlocal/refs/heads/main/security/ownlocal-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Advertising
- Local Media
- Digital Advertising
- Marketing
- Newspapers
- AdTech
- Print to Digital
- Business Listings
- Local Business Data
- Ad Reporting
- Publishers
---
