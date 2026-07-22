---
api_specs:
- filename: nym-technologies-nym-api-openapi.json
  format: json
  label: Nym API
  slug: nym-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nym-technologies/refs/heads/main/openapi/nym-technologies-nym-api-openapi.json
- filename: nym-technologies-node-status-api-openapi.json
  format: json
  label: Node Status API
  slug: node-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nym-technologies/refs/heads/main/openapi/nym-technologies-node-status-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nym.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nymtech.net
  spf: true
hosts:
- cert_expires: Oct 17 19:08:00 2026 GMT
  host: nym.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 06:55:22 2026 GMT
  host: validator.nymtech.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 11:59:49 2026 GMT
  host: mainnet-node-status-api.nymtech.cc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nym Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nym Technologies, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nym Technologies
provider_slug: nym-technologies
slug: nym-technologies-domain-security
source_filename: nym-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nym.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 19:08:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: validator.nymtech.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:55:22 2026 GMT\n  hsts: null\n- host: mainnet-node-status-api.nymtech.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 11:59:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nym.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nymtech.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nym-technologies/refs/heads/main/security/nym-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Privacy
- VPN
- Mixnet
- Cryptography
- Decentralized
- Networking
- Web3
- Blockchain
- Anonymity
- Zero Knowledge
- Security
---
