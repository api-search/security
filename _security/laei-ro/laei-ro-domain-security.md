---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: laei.ro
  spf: true
hosts:
- cert_expires: Jan 22 21:27:22 2027 GMT
  host: laei.ro
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: laei-ro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for laei-ro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: laei-ro
provider_slug: laei-ro
slug: laei-ro-domain-security
source_filename: laei-ro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laei.ro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 21:27:22 2027 GMT\n  hsts: false\ndomains:\n- domain: laei.ro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/laei-ro/security/laei-ro-domain-security.yml
summary_line: TLSv1.3
tags:
- Servers
- Skins
- MODS
- Tools
- Community
---
