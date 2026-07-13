---
api_specs:
- filename: sketchfab-data-api-openapi.yml
  format: yaml
  label: Sketchfab Data API
  slug: sketchfab-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-data-api-openapi.yml
- filename: sketchfab-download-api-openapi.yml
  format: yaml
  label: Sketchfab Download API
  slug: sketchfab-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-download-api-openapi.yml
- filename: sketchfab-oembed-api-openapi.yml
  format: yaml
  label: Sketchfab oEmbed API
  slug: sketchfab-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-oembed-api-openapi.yml
- filename: sketchfab-oauth-api-openapi.yml
  format: yaml
  label: Sketchfab OAuth 2.0 API
  slug: sketchfab-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-oauth-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sketchfab.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: sketchfab.com
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: api.sketchfab.com
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sketchfab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sketchfab, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sketchfab
provider_slug: sketchfab
slug: sketchfab-domain-security
source_filename: sketchfab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sketchfab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 604800\n- host: api.sketchfab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: sketchfab.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/security/sketchfab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- 3D
- Models
- Marketplace
- Viewer
- WebGL
- glTF
- AR
- VR
- Creative
- Epic Games
---
