---
api_specs:
- filename: roblox-engine-api-assets-api-openapi.yml
  format: yaml
  label: Roblox Engine API Assets API
  slug: roblox-engine-api-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/openapi/roblox-engine-api-assets-api-openapi.yml
- filename: roblox-engine-api-data-stores-api-openapi.yml
  format: yaml
  label: Roblox Engine API Data Stores API
  slug: roblox-engine-api-data-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/openapi/roblox-engine-api-data-stores-api-openapi.yml
- filename: roblox-engine-api-groups-api-openapi.yml
  format: yaml
  label: Roblox Engine API Groups API
  slug: roblox-engine-api-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/openapi/roblox-engine-api-groups-api-openapi.yml
- filename: roblox-engine-api-messaging-api-openapi.yml
  format: yaml
  label: Roblox Engine API Messaging API
  slug: roblox-engine-api-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/openapi/roblox-engine-api-messaging-api-openapi.yml
- filename: roblox-engine-api-places-api-openapi.yml
  format: yaml
  label: Roblox Engine API Places API
  slug: roblox-engine-api-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/openapi/roblox-engine-api-places-api-openapi.yml
- filename: roblox-engine-api-universes-api-openapi.yml
  format: yaml
  label: Roblox Engine API Universes API
  slug: roblox-engine-api-universes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/openapi/roblox-engine-api-universes-api-openapi.yml
- filename: roblox-engine-api-users-api-openapi.yml
  format: yaml
  label: Roblox Engine API Users API
  slug: roblox-engine-api-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/openapi/roblox-engine-api-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: roblox.com
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: www.roblox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: create.roblox.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: apis.roblox.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roblox Engine Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roblox Engine API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Roblox Engine API
provider_slug: roblox-engine-api
slug: roblox-engine-api-domain-security
source_filename: roblox-engine-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.roblox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: create.roblox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apis.roblox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: roblox.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/security/roblox-engine-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gaming
- Game Development
- Metaverse
- Roblox
- Open Cloud
---
