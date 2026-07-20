---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sovrun.org
  spf: false
hosts:
- cert_expires: Aug 21 09:30:15 2026 GMT
  host: www.sovrun.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 07:30:11 2026 GMT
  host: docs.sovrun.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.ready-gamer.sovrun.org
  https: false
kind: domain-security
layout: security
method: probed
name: Breederdao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BreederDAO, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: BreederDAO
provider_slug: breederdao
slug: breederdao-domain-security
source_filename: breederdao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sovrun.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 09:30:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sovrun.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 07:30:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ready-gamer.sovrun.org\n  https: false\ndomains:\n- domain: sovrun.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breederdao/refs/heads/main/security/breederdao-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Web3
- Blockchain
- Gaming
- NFT
- Autonomous Worlds
- AI Agents
- Developer Tools
---
