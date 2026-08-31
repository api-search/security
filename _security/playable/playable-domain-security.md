---
api_specs:
- filename: playable-campaigns-api-openapi.yml
  format: yaml
  label: Playable Campaigns API
  slug: playable-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/openapi/playable-campaigns-api-openapi.yml
- filename: playable-media-api-openapi.yml
  format: yaml
  label: Playable Media API
  slug: playable-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/openapi/playable-media-api-openapi.yml
- filename: playable-oauth-api-openapi.yml
  format: yaml
  label: Playable OAUTH API
  slug: playable-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/openapi/playable-oauth-api-openapi.yml
- filename: playable-user-api-openapi.yml
  format: yaml
  label: Playable User API
  slug: playable-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/openapi/playable-user-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:tech-services+caareport@playable.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: playable.com
  spf: true
hosts:
- cert_expires: Oct 25 12:25:11 2026 GMT
  host: playable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: api.playable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: sdk.playable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Playable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Playable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Playable
provider_slug: playable
slug: playable-domain-security
source_filename: playable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: playable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 12:25:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.playable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sdk.playable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: playable.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:tech-services+caareport@playable.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/security/playable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- marketing-gamification
- interactive-marketing
- campaign-management
- zero-party-data
- lead-generation
- loyalty
- martech
- Webhook
- Authentication
---
