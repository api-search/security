---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bloom.co
  spf: true
hosts:
- cert_expires: Sep 20 13:38:34 2026 GMT
  host: bloom.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bloom
provider_slug: bloom
slug: bloom-domain-security
source_filename: bloom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bloom.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 13:38:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bloom.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloom/refs/heads/main/security/bloom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Identity
- Verifiable Credentials
- Decentralized Identity
- Credit Scoring
- Blockchain
- Ethereum
- Self-Sovereign Identity
- Discontinued
---
