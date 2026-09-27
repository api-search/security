---
api_specs:
- filename: aztecprotocol-openapi-generated.yml
  format: yaml
  label: Aztecprotocol API
  slug: aztecprotocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aztecprotocol/refs/heads/main/openapi/_ae-authored/aztecprotocol-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aztec.network
  spf: true
hosts:
- cert_expires: Nov 25 13:44:48 2026 GMT
  host: aztec.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aztecprotocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aztecprotocol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Aztecprotocol
provider_slug: aztecprotocol
slug: aztecprotocol-domain-security
source_filename: aztecprotocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aztec.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 13:44:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aztec.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aztecprotocol/refs/heads/main/security/aztecprotocol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Privacy
- zkRollup
- Ethereum
- Decentralized
---
