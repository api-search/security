---
api_specs:
- filename: atproto-com-atproto-openapi.yml
  format: yaml
  label: AT Protocol Core API (com.atproto)
  slug: com-atproto
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-com-atproto-openapi.yml
- filename: atproto-app-bsky-openapi.yml
  format: yaml
  label: Bluesky Application API (app.bsky)
  slug: app-bsky
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atproto/refs/heads/main/openapi/atproto-app-bsky-openapi.yml
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
- Open Source
- Bluesky
- Fediverse
- Identity
- XRPC
- Lexicon
---
