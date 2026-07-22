---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: matchday.com
  spf: true
hosts:
- cert_expires: Sep 20 02:05:32 2026 GMT
  host: matchday.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Matchday Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matchday, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Matchday
provider_slug: matchday
slug: matchday-domain-security
source_filename: matchday-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: matchday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 02:05:32 2026 GMT\n  hsts: false\ndomains:\n- domain: matchday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matchday/refs/heads/main/security/matchday-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sports
- Football
- Soccer
- Collectibles
- Digital Collectibles
- Gaming
- Consumer
- Mobile
---
