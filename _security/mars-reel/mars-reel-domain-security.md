---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marsreel.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tfiom.com
  spf: true
hosts:
- cert_expires: Oct 13 18:47:06 2026 GMT
  host: marsreel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:32:32 2026 GMT
  host: tfiom.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mars Reel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mars Reel, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mars Reel
provider_slug: mars-reel
slug: mars-reel-domain-security
source_filename: mars-reel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marsreel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 18:47:06 2026 GMT\n  hsts: false\n- host: tfiom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:32:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: marsreel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tfiom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mars-reel/refs/heads/main/security/mars-reel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sports
- Media
- Streaming
- Video
- Youth Sports
- Entertainment
- Membership
---
