---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jigsawapps.com
  spf: true
hosts:
- cert_expires: Jan  3 21:03:46 2027 GMT
  host: jigsawapps.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jigsaw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jigsaw, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jigsaw
provider_slug: jigsawapps-com
slug: jigsawapps-com-domain-security
source_filename: jigsawapps-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jigsawapps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 21:03:46 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: jigsawapps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jigsawapps-com/security/jigsawapps-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- Collaboration
- Artificial Intelligence
- Chatbots
- Productivity
---
