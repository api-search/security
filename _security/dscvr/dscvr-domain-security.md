---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dscvr.one
  spf: true
hosts:
- cert_expires: Sep 23 06:33:45 2026 GMT
  host: dscvr.one
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 22:12:47 2026 GMT
  host: docs.dscvr.one
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 03:27:03 2026 GMT
  host: api.dscvr.one
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dscvr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DSCVR, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DSCVR
provider_slug: dscvr
slug: dscvr-domain-security
source_filename: dscvr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dscvr.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:33:45 2026 GMT\n  hsts: false\n- host: docs.dscvr.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 22:12:47 2026 GMT\n  hsts: false\n- host: api.dscvr.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:27:03 2026 GMT\n  hsts: null\ndomains:\n- domain: dscvr.one\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dscvr/refs/heads/main/security/dscvr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Social
- Web3
- GraphQL
- Blockchain
- Solana
- Internet Computer
- SocialFi
- Social Graph
- Developer Platform
---
