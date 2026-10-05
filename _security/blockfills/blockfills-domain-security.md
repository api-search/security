---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blockfills.com
  spf: true
hosts:
- cert_expires: Nov 18 18:47:40 2026 GMT
  host: www.blockfills.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blockfills Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlockFills, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BlockFills
provider_slug: blockfills
slug: blockfills-domain-security
source_filename: blockfills-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blockfills.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 18:47:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blockfills.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockfills/refs/heads/main/security/blockfills-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Trading
- Fintech
---
