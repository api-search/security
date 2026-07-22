---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: divestudios.io
  spf: false
hosts:
- cert_expires: Sep 14 18:13:16 2026 GMT
  host: divestudios.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dive Studios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DIVE studios, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: DIVE studios
provider_slug: dive-studios
slug: dive-studios-domain-security
source_filename: dive-studios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: divestudios.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:13:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: divestudios.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dive-studios/refs/heads/main/security/dive-studios-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- K-Entertainment
- Advertising
- Influencer Marketing
- Content
- Entertainment
---
