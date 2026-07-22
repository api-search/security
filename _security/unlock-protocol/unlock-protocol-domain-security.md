---
api_specs:
- filename: unlock-protocol-locksmith-openapi.yml
  format: yaml
  label: Unlock Locksmith API
  slug: unlock-locksmith-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock-protocol/refs/heads/main/openapi/unlock-protocol-locksmith-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: unlock-protocol.com
  spf: true
hosts:
- cert_expires: Aug 29 22:37:13 2026 GMT
  host: unlock-protocol.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 22:37:13 2026 GMT
  host: locksmith.unlock-protocol.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 16:31:27 2026 GMT
  host: staging-locksmith.unlock-protocol.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unlock Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unlock Protocol, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Unlock Protocol
provider_slug: unlock-protocol
slug: unlock-protocol-domain-security
source_filename: unlock-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unlock-protocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 22:37:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: locksmith.unlock-protocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 22:37:13 2026 GMT\n  hsts: false\n- host: staging-locksmith.unlock-protocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 16:31:27 2026 GMT\n  hsts: false\ndomains:\n- domain: unlock-protocol.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unlock-protocol/refs/heads/main/security/unlock-protocol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Memberships
- Subscriptions
- NFT
- Ticketing
- Web3
- Payments
---
