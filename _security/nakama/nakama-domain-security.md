---
api_specs:
- filename: nakama-openapi.yml
  format: yaml
  label: Nakama Authentication API
  slug: nakama-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-openapi.yml
- filename: nakama-openapi.yml
  format: yaml
  label: Nakama Account API
  slug: nakama-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-openapi.yml
- filename: nakama-openapi.yml
  format: yaml
  label: Nakama Friends and Groups API
  slug: nakama-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-openapi.yml
- filename: nakama-openapi.yml
  format: yaml
  label: Nakama Storage API
  slug: nakama-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-openapi.yml
- filename: nakama-openapi.yml
  format: yaml
  label: Nakama Leaderboards and Tournaments API
  slug: nakama-leaderboards-tournaments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-openapi.yml
- filename: nakama-openapi.yml
  format: yaml
  label: Nakama Notifications API
  slug: nakama-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-openapi.yml
- filename: nakama-openapi.yml
  format: yaml
  label: Nakama RPC and Runtime API
  slug: nakama-rpc-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-openapi.yml
- filename: nakama-asyncapi.yml
  format: yaml
  label: Nakama Realtime Socket API
  slug: nakama-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/asyncapi/nakama-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: heroiclabs.com
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: heroiclabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Nakama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nakama, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Nakama
provider_slug: nakama
slug: nakama-domain-security
source_filename: nakama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heroiclabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: heroiclabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/security/nakama-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Gaming
- Game Backend
- Backend
- Realtime
- Multiplayer
- Matchmaking
- Leaderboards
- Social
- Open Source
---
