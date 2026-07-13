---
api_specs:
- filename: at-protocol-openapi.yml
  format: yaml
  label: AT Protocol XRPC API
  slug: atproto-xrpc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-protocol/refs/heads/main/openapi/at-protocol-openapi.yml
- filename: at-protocol-asyncapi.yml
  format: yaml
  label: AT Protocol Relay & Firehose
  slug: relay-firehose
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-protocol/refs/heads/main/asyncapi/at-protocol-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atproto.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: bsky.network
  spf: false
hosts:
- cert_expires: Sep 17 18:20:39 2026 GMT
  host: atproto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 10:23:29 2026 GMT
  host: bsky.network
  hsts: null
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
name: At Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AT Protocol, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AT Protocol
provider_slug: at-protocol
slug: at-protocol-domain-security
source_filename: at-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atproto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 18:20:39 2026 GMT\n  hsts: false\n- host: bsky.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:23:29 2026 GMT\n  hsts: null\n- host: docs.bsky.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 02:04:29 2026 GMT\n  hsts: false\ndomains:\n- domain: atproto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bsky.network\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/at-protocol/refs/heads/main/security/at-protocol-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AT Protocol
- atproto
- Bluesky
- Federation
- Decentralized Social
- Social Networking
- DID
- Lexicon
- XRPC
- PDS
- Relay
- AppView
- Open Protocol
---
