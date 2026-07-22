---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: peerby.com
  spf: true
hosts:
- cert_expires: Sep 10 23:38:43 2026 GMT
  host: peerby.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peerby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peerby, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Peerby
provider_slug: peerby
slug: peerby-domain-security
source_filename: peerby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: peerby.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:38:43 2026 GMT\n  hsts: false\ndomains:\n- domain: peerby.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peerby/refs/heads/main/security/peerby-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sharing Economy
- Peer to Peer
- Marketplace
- Rental
- Sustainability
- Consumer
- Netherlands
---
