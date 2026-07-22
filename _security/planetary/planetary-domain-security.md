---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: planetary.social
  spf: true
hosts:
- cert_expires: Oct  4 04:12:14 2026 GMT
  host: planetary.social
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Planetary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Planetary, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Planetary
provider_slug: planetary
slug: planetary-domain-security
source_filename: planetary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: planetary.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:12:14 2026 GMT\n  hsts: false\ndomains:\n- domain: planetary.social\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planetary/refs/heads/main/security/planetary-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Social
- Social Media
- Decentralized
- Peer-to-Peer
- Scuttlebutt
- Nostr
- Open Source
- Protocol
- iOS
---
