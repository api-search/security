---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: common.xyz
  spf: true
hosts:
- cert_expires: Aug 20 16:01:06 2026 GMT
  host: common.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Commonwealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commonwealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Commonwealth
provider_slug: commonwealth
slug: commonwealth-domain-security
source_filename: commonwealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: common.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 16:01:06 2026 GMT\n  hsts: false\ndomains:\n- domain: common.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commonwealth/refs/heads/main/security/commonwealth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Web3
- Governance
- DAO
- Blockchain
- Onchain Communities
- Forums
- Launchpad
- Coordination
- Crypto
---
