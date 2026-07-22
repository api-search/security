---
api_specs:
- filename: proof-of-play-vrf-openapi.json
  format: json
  label: Proof of Play vRNG API
  slug: proof-of-play-vrng-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proof-of-play/refs/heads/main/openapi/proof-of-play-vrf-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: proofofplay.com
  spf: true
hosts:
- cert_expires: Sep  8 04:00:19 2026 GMT
  host: staging.vrf.proofofplay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Proof Of Play Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proof of Play, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Proof of Play
provider_slug: proof-of-play
slug: proof-of-play-domain-security
source_filename: proof-of-play-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: staging.vrf.proofofplay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 04:00:19 2026 GMT\n  hsts: null\ndomains:\n- domain: proofofplay.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proof-of-play/refs/heads/main/security/proof-of-play-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Gaming
- Blockchain
- Web3
- Randomness
- Onchain Infrastructure
- NFT
- Developer Services
---
