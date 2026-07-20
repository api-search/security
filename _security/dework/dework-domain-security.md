---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dework.xyz
  spf: true
hosts:
- cert_expires: Sep 24 06:05:44 2026 GMT
  host: dework.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dework Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dework, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dework
provider_slug: dework
slug: dework-domain-security
source_filename: dework-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dework.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 06:05:44 2026 GMT\n  hsts: false\ndomains:\n- domain: dework.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dework/refs/heads/main/security/dework-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Crypto Tools
- Web3
- DAO
- Task Management
- Bounties
- Project Management
- Decentralized Work
---
