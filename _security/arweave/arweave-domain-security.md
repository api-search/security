---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Arweave HTTP Node API
  slug: arweave-http-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arweave/refs/heads/main/openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arweave.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: arweave.net
  spf: false
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: www.arweave.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 16:18:24 2026 GMT
  host: docs.arweave.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 11:43:36 2026 GMT
  host: arweave.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arweave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arweave, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arweave
provider_slug: arweave
slug: arweave-domain-security
source_filename: arweave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arweave.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: false\n- host: docs.arweave.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 16:18:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: arweave.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 11:43:36 2026 GMT\n  hsts: false\ndomains:\n- domain: arweave.org\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: arweave.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arweave/refs/heads/main/security/arweave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Decentralized Storage
- Blockchain
- Permaweb
- Web3
- Data Storage
- GraphQL
---
