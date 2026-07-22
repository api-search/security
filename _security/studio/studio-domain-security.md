---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: s-tud.io
  spf: true
hosts:
- cert_expires: Sep 14 08:25:01 2026 GMT
  host: s-tud.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Studio
provider_slug: studio
slug: studio-domain-security
source_filename: studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: s-tud.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:25:01 2026 GMT\n  hsts: false\ndomains:\n- domain: s-tud.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/studio/refs/heads/main/security/studio-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Art
- Creative
- Software
- Design
- Media
---
