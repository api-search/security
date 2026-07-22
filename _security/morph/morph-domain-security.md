---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: morphl2.io
  spf: true
hosts:
- cert_expires: Aug 26 06:49:57 2026 GMT
  host: www.morphl2.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Morph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Morph, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Morph
provider_slug: morph
slug: morph-domain-security
source_filename: morph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.morphl2.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:49:57 2026 GMT\n  hsts: false\ndomains:\n- domain: morphl2.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morph/refs/heads/main/security/morph-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- Blockchain
- Layer 2
- Ethereum
- zkEVM
- Web3
- Developer Tools
---
