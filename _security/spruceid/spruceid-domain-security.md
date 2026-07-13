---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: SpruceID DIDKit HTTP API
  slug: spruceid-didkit-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/spruceid/didkit-http/main/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spruceid.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: spruceid.dev
  spf: true
hosts:
- cert_expires: Aug 13 10:18:08 2026 GMT
  host: spruceid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 14:33:47 2026 GMT
  host: spruceid.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 09:32:19 2026 GMT
  host: eips.ethereum.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spruceid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpruceID, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SpruceID
provider_slug: spruceid
slug: spruceid-domain-security
source_filename: spruceid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spruceid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 10:18:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: spruceid.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:33:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eips.ethereum.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 09:32:19 2026 GMT\n  hsts: false\ndomains:\n- domain: spruceid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: spruceid.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spruceid/refs/heads/main/security/spruceid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Decentralized Identity
- Verifiable Credentials
- DIDs
- Sign-In with Ethereum
- Identity Wallet
- Government
- OpenID Connect
- W3C Standards
---
