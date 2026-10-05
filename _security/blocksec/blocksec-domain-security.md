---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: blocksec.com
  spf: true
hosts:
- cert_expires: Dec 28 04:58:07 2026 GMT
  host: blocksec.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blocksec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlockSec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BlockSec
provider_slug: blocksec
slug: blocksec-domain-security
source_filename: blocksec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blocksec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 04:58:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blocksec.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blocksec/refs/heads/main/security/blocksec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Blockchain
- Web3
- Compliance
- Auditing
---
