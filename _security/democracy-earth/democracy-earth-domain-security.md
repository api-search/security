---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: democracy.earth
  spf: true
hosts:
- cert_expires: Sep  9 16:12:08 2026 GMT
  host: democracy.earth
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Democracy Earth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Democracy Earth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Democracy Earth
provider_slug: democracy-earth
slug: democracy-earth-domain-security
source_filename: democracy-earth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: democracy.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 16:12:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: democracy.earth\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/democracy-earth/refs/heads/main/security/democracy-earth-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Governance
- Voting
- Blockchain
- Democracy
- Decentralized Identity
- Open Source
- Web3
- Nonprofit
---
