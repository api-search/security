---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: websummit.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: collisionconf.com
  spf: true
hosts:
- cert_expires: Sep 21 06:27:32 2026 GMT
  host: vancouver.websummit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 00:56:51 2026 GMT
  host: collisionconf.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 00:56:51 2026 GMT
  host: speakers.collisionconf.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Collision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Collision (now Web Summit Vancouver), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Collision (now Web Summit Vancouver)
provider_slug: collision
slug: collision-domain-security
source_filename: collision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vancouver.websummit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 06:27:32 2026 GMT\n  hsts: false\n- host: collisionconf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:56:51 2026 GMT\n  hsts: false\n- host: speakers.collisionconf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:56:51 2026 GMT\n  hsts: false\ndomains:\n- domain: websummit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: collisionconf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collision/refs/heads/main/security/collision-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Conferences
- Events
- Historical
- Rebrand
- Startups
- Technology
- Web Summit
---
