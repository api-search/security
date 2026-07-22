---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pixelworks.com
  spf: true
hosts:
- cert_expires: Oct  2 23:01:13 2026 GMT
  host: www.pixelworks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixelworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixelworks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pixelworks
provider_slug: pixelworks
slug: pixelworks-domain-security
source_filename: pixelworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pixelworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:01:13 2026 GMT\n  hsts: false\ndomains:\n- domain: pixelworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixelworks/refs/heads/main/security/pixelworks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Semiconductors
- Video Processing
- Image Processing
- Visual Processing
- Displays
- Hardware
- Integrated Circuits
---
