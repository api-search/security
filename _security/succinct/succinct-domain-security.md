---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: succinct.xyz
  spf: true
hosts:
- cert_expires: Oct 12 11:12:38 2026 GMT
  host: succinct.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Succinct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Succinct, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Succinct
provider_slug: succinct
slug: succinct-domain-security
source_filename: succinct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: succinct.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 11:12:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: succinct.xyz\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/succinct/refs/heads/main/security/succinct-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Infrastructure
- Zero-Knowledge Proofs
- zkVM
- Blockchain
- Ethereum
- Cryptography
- Developer Tools
- Prover Network
- gRPC
---
