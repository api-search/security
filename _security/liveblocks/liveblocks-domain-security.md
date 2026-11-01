---
api_specs:
- filename: liveblocks-comments-api-openapi.yml
  format: yaml
  label: Liveblocks Comments API
  slug: liveblocks-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-comments-api-openapi.yml
- filename: liveblocks-storage-api-openapi.yml
  format: yaml
  label: Liveblocks Storage API
  slug: liveblocks-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-storage-api-openapi.yml
- filename: liveblocks-yjs-api-openapi.yml
  format: yaml
  label: Liveblocks Yjs API
  slug: liveblocks-yjs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-yjs-api-openapi.yml
- filename: liveblocks-ai-api-openapi.yml
  format: yaml
  label: Liveblocks AI API
  slug: liveblocks-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-ai-api-openapi.yml
- filename: liveblocks-auth-api-openapi.yml
  format: yaml
  label: Liveblocks Auth API
  slug: liveblocks-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-auth-api-openapi.yml
- filename: liveblocks-feeds-api-openapi.yml
  format: yaml
  label: Liveblocks Feeds API
  slug: liveblocks-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-feeds-api-openapi.yml
- filename: liveblocks-groups-api-openapi.yml
  format: yaml
  label: Liveblocks Groups API
  slug: liveblocks-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-groups-api-openapi.yml
- filename: liveblocks-management-api-openapi.yml
  format: yaml
  label: Liveblocks Management API
  slug: liveblocks-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-management-api-openapi.yml
- filename: liveblocks-notifications-api-openapi.yml
  format: yaml
  label: Liveblocks Notifications API
  slug: liveblocks-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-notifications-api-openapi.yml
- filename: liveblocks-room-api-openapi.yml
  format: yaml
  label: Liveblocks Room API
  slug: liveblocks-room-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-room-api-openapi.yml
- filename: liveblocks-version-history-api-openapi.yml
  format: yaml
  label: Liveblocks Version History API
  slug: liveblocks-version-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liveblocks/openapi/liveblocks-version-history-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: liveblocks.io
  spf: true
hosts:
- cert_expires: Sep 29 03:38:26 2026 GMT
  host: liveblocks.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 20:18:32 2026 GMT
  host: api.liveblocks.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Liveblocks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liveblocks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Liveblocks
provider_slug: liveblocks
slug: liveblocks-domain-security
source_filename: liveblocks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liveblocks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:38:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.liveblocks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 20:18:32 2026 GMT\n  hsts: null\ndomains:\n- domain: liveblocks.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/liveblocks/security/liveblocks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Time
- Collaboration
- Multiplayer
- Presence
- CRDT
- Yjs
- Comments
- Threads
- Notification
- WebSocket
---
