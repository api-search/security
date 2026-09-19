---
api_specs:
- filename: upland-accounts-api-openapi.yml
  format: yaml
  label: Upland Accounts API
  slug: upland-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-accounts-api-openapi.yml
- filename: upland-application-usage-api-openapi.yml
  format: yaml
  label: Upland Application Usage API
  slug: upland-application-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-application-usage-api-openapi.yml
- filename: upland-authentication-api-openapi.yml
  format: yaml
  label: Upland Authentication API
  slug: upland-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-authentication-api-openapi.yml
- filename: upland-chain-api-openapi.yml
  format: yaml
  label: Upland Chain API
  slug: upland-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-chain-api-openapi.yml
- filename: upland-dev-shops-api-openapi.yml
  format: yaml
  label: Upland Dev Shops API
  slug: upland-dev-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-dev-shops-api-openapi.yml
- filename: upland-escrow-containers-api-openapi.yml
  format: yaml
  label: Upland Escrow Containers API
  slug: upland-escrow-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-escrow-containers-api-openapi.yml
- filename: upland-generic-api-openapi.yml
  format: yaml
  label: Upland Generic API
  slug: upland-generic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-generic-api-openapi.yml
- filename: upland-history-api-openapi.yml
  format: yaml
  label: Upland History API
  slug: upland-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-history-api-openapi.yml
- filename: upland-hyperion-history-api-for-upland-chain-api-openapi.yml
  format: yaml
  label: Upland Hyperion History API For UPLAND Chain API
  slug: upland-hyperion-history-api-for-upland-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-hyperion-history-api-for-upland-chain-api-openapi.yml
- filename: upland-internal-api-openapi.yml
  format: yaml
  label: Upland Internal API
  slug: upland-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-internal-api-openapi.yml
- filename: upland-node-api-openapi.yml
  format: yaml
  label: Upland Node API
  slug: upland-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-node-api-openapi.yml
- filename: upland-state-api-openapi.yml
  format: yaml
  label: Upland State API
  slug: upland-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-state-api-openapi.yml
- filename: upland-stats-api-openapi.yml
  format: yaml
  label: Upland Stats API
  slug: upland-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-stats-api-openapi.yml
- filename: upland-status-api-openapi.yml
  format: yaml
  label: Upland Status API
  slug: upland-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-status-api-openapi.yml
- filename: upland-system-api-openapi.yml
  format: yaml
  label: Upland System API
  slug: upland-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-system-api-openapi.yml
- filename: upland-tournaments-api-openapi.yml
  format: yaml
  label: Upland Tournaments API
  slug: upland-tournaments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-tournaments-api-openapi.yml
- filename: upland-upland-user-api-openapi.yml
  format: yaml
  label: Upland Upland User API
  slug: upland-upland-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-upland-user-api-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: upland.me
  spf: true
hosts:
- cert_expires: Nov 16 15:33:01 2026 GMT
  host: upland.me
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 11:02:09 2026 GMT
  host: docs.developers.upland.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 16:49:13 2026 GMT
  host: api.prod.upland.me
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Upland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upland, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Upland
provider_slug: upland
slug: upland-domain-security
source_filename: upland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upland.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 15:33:01 2026 GMT\n  hsts: false\n- host: docs.developers.upland.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 11:02:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.prod.upland.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 16:49:13 2026 GMT\n  hsts: null\ndomains:\n- domain: upland.me\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/security/upland-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Metaverse
- Web3
- Gaming
- Blockchain
- NFT
- Virtual Real Estate
- Digital Assets
- Escrow
- Tournaments
- Antelope
- Webhook
- Developer Platform
---
