---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: secondhome.io
  spf: true
hosts:
- cert_expires: Sep 17 17:35:16 2026 GMT
  host: secondhome.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Second Home Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Second Home, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Second Home
provider_slug: second-home
slug: second-home-domain-security
source_filename: second-home-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: secondhome.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 17:35:16 2026 GMT\n  hsts: false\ndomains:\n- domain: secondhome.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/second-home/refs/heads/main/security/second-home-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Future Of Work
- Coworking
- Workspace
- Flexible Office
- Cultural Venue
- Real Estate
- Community
---
