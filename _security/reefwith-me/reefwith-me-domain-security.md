---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: reefwith.me
  spf: false
hosts:
- cert_expires: Jan  7 15:08:44 2027 GMT
  host: reefwith.me
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: reef Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for reef, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: reef
provider_slug: reefwith-me
slug: reefwith-me-domain-security
source_filename: reefwith-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reefwith.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 15:08:44 2027 GMT\n  hsts: false\ndomains:\n- domain: reefwith.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/reefwith-me/security/reefwith-me-domain-security.yml
summary_line: TLSv1.3
tags:
- AI
- Memory
- Collaboration
- Privacy
- Invitation
---
