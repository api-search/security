---
api_specs:
- filename: iconik-openapi.yml
  format: yaml
  label: iconik Assets API
  slug: iconik-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iconik/refs/heads/main/openapi/iconik-openapi.yml
- filename: iconik-openapi.yml
  format: yaml
  label: iconik Collections API
  slug: iconik-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iconik/refs/heads/main/openapi/iconik-openapi.yml
- filename: iconik-openapi.yml
  format: yaml
  label: iconik Metadata API
  slug: iconik-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iconik/refs/heads/main/openapi/iconik-openapi.yml
- filename: iconik-openapi.yml
  format: yaml
  label: iconik Search API
  slug: iconik-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iconik/refs/heads/main/openapi/iconik-openapi.yml
- filename: iconik-openapi.yml
  format: yaml
  label: iconik Files API
  slug: iconik-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iconik/refs/heads/main/openapi/iconik-openapi.yml
- filename: iconik-openapi.yml
  format: yaml
  label: iconik Jobs API
  slug: iconik-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iconik/refs/heads/main/openapi/iconik-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "'digicert.com"
  - 0 issue "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: iconik.io
  spf: true
hosts:
- cert_expires: Aug 30 17:36:20 2026 GMT
  host: www.iconik.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 08:52:58 2026 GMT
  host: app.iconik.io
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 21:06:51 2026 GMT
  host: eu.iconik.io
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iconik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iconik, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: iconik
provider_slug: iconik
slug: iconik-domain-security
source_filename: iconik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iconik.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 17:36:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.iconik.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 08:52:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: eu.iconik.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 21:06:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: iconik.io\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"'digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iconik/refs/heads/main/security/iconik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Media Asset Management
- MAM
- Video
- Media
- Cloud Storage
- Metadata
- Search
- Assets
---
