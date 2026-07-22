---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: snow.me
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: kajicam.com
  spf: false
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: b612.snow.me
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: kajicam.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: B612 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for B612, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: B612
provider_slug: b612
slug: b612-domain-security
source_filename: b612-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: b612.snow.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: false\n- host: kajicam.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: snow.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: kajicam.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/b612/refs/heads/main/security/b612-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Technology
- Photography
- Mobile Applications
- Camera
- Consumer Applications
- Video Editing
- Augmented Reality
- China
- South Korea
---
