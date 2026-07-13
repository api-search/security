---
api_specs:
- filename: api.yaml
  format: yaml
  label: Polygon ID Issuer Node API
  slug: polygon-id-issuer-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/0xPolygonID/issuer-node/main/api/api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: privado.id
  spf: true
hosts:
- cert_expires: Sep 11 05:24:25 2026 GMT
  host: www.privado.id
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 06:36:59 2026 GMT
  host: docs.privado.id
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 06:36:59 2026 GMT
  host: issuer-node-core-api-testing.privado.id
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polygon Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polygon ID, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Polygon ID
provider_slug: polygon-id
slug: polygon-id-domain-security
source_filename: polygon-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.privado.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:24:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.privado.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:36:59 2026 GMT\n  hsts: false\n- host: issuer-node-core-api-testing.privado.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:36:59 2026 GMT\n  hsts: null\ndomains:\n- domain: privado.id\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/security/polygon-id-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Identity
- Verifiable Credentials
- Zero-Knowledge Proofs
- Self-Sovereign Identity
- Decentralized Identity
- Blockchain
- Web3
- KYC
---
