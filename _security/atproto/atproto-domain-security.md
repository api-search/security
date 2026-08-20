---
api_specs:
- filename: atproto-actor-api-openapi.yml
  format: yaml
  label: AT Protocol actor API
  slug: atproto-actor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-actor-api-openapi.yml
- filename: atproto-feed-api-openapi.yml
  format: yaml
  label: AT Protocol feed API
  slug: atproto-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-feed-api-openapi.yml
- filename: atproto-graph-api-openapi.yml
  format: yaml
  label: AT Protocol graph API
  slug: atproto-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-graph-api-openapi.yml
- filename: atproto-identity-api-openapi.yml
  format: yaml
  label: AT Protocol identity API
  slug: atproto-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-identity-api-openapi.yml
- filename: atproto-notification-api-openapi.yml
  format: yaml
  label: AT Protocol notification API
  slug: atproto-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-notification-api-openapi.yml
- filename: atproto-repo-api-openapi.yml
  format: yaml
  label: AT Protocol repo API
  slug: atproto-repo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-repo-api-openapi.yml
- filename: atproto-server-api-openapi.yml
  format: yaml
  label: AT Protocol server API
  slug: atproto-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-server-api-openapi.yml
- filename: atproto-sync-api-openapi.yml
  format: yaml
  label: AT Protocol sync API
  slug: atproto-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-sync-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atproto.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bsky.social
  spf: false
hosts:
- cert_expires: Sep 17 18:20:39 2026 GMT
  host: atproto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: bsky.social
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 02:04:29 2026 GMT
  host: docs.bsky.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atproto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AT Protocol, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AT Protocol
provider_slug: atproto
slug: atproto-domain-security
source_filename: atproto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atproto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 18:20:39 2026 GMT\n  hsts: false\n- host: bsky.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\n- host: docs.bsky.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 02:04:29 2026 GMT\n  hsts: false\ndomains:\n- domain: atproto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bsky.social\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/security/atproto-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Social Networking
- Decentralized
- Federated
- Open-Source
- Bluesky
- Fediverse
- Identity
- XRPC
- Lexicon
---
