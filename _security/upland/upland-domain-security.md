---
api_specs:
- filename: upland-developers-api-openapi.json
  format: json
  label: Upland Developers API
  slug: upland-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-developers-api-openapi.json
- filename: upland-appchain-history-swagger.json
  format: json
  label: Upland Appchain History & Chain API
  slug: upland-appchain-history-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-appchain-history-swagger.json
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
- Webhooks
- Developer Platform
---
