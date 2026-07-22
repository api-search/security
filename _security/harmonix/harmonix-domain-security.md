---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: harmonixmusic.com
  spf: true
hosts:
- cert_expires: Sep  8 17:32:04 2026 GMT
  host: www.harmonixmusic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harmonix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harmonix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Harmonix
provider_slug: harmonix
slug: harmonix-domain-security
source_filename: harmonix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.harmonixmusic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 17:32:04 2026 GMT\n  hsts: false\ndomains:\n- domain: harmonixmusic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harmonix/refs/heads/main/security/harmonix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Music Games
- Rhythm Games
- Video Games
- Game Development
- Entertainment
---
