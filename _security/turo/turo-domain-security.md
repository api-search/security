---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: turo.com
  spf: true
hosts:
- cert_expires: Oct  7 03:48:18 2026 GMT
  host: turo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Turo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Turo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Turo
provider_slug: turo
slug: turo-domain-security
source_filename: turo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: turo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:48:18 2026 GMT\n  hsts: false\ndomains:\n- domain: turo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turo/refs/heads/main/security/turo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Car Sharing
- Peer To Peer
- Marketplace
- Mobility
- Travel
- Transportation
- Car Rental
- Connected Car
- Automotive
- Hosts
- Trips
---
