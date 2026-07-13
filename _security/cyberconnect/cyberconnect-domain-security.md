---
api_specs:
- filename: openapi.yml
  format: yaml
  label: CyberConnect GraphQL API
  slug: cyberconnect-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberconnect/refs/heads/main/openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cyber.co
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vercel.app
  spf: true
hosts:
- cert_expires: Aug 21 11:18:34 2026 GMT
  host: cyber.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 13:27:56 2026 GMT
  host: cyberconnect-docs-v2.vercel.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.cybertino.io
  https: false
kind: domain-security
layout: security
method: probed
name: Cyberconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CyberConnect, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CyberConnect
provider_slug: cyberconnect
slug: cyberconnect-domain-security
source_filename: cyberconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cyber.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 11:18:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cyberconnect-docs-v2.vercel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:27:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cybertino.io\n  https: false\ndomains:\n- domain: cyber.co\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: vercel.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyberconnect/refs/heads/main/security/cyberconnect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Social Graph
- Decentralized
- GraphQL
- Blockchain
- Social Network
- Identity
---
