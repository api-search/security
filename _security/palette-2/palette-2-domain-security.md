---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: palettetechnology.com
  spf: false
hosts:
- cert_expires: Sep 27 22:48:33 2026 GMT
  host: palettetechnology.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 07:17:59 2026 GMT
  host: studio.palettetechnology.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Palette 2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Palette 2, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Palette 2
provider_slug: palette-2
slug: palette-2-domain-security
source_filename: palette-2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: palettetechnology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 22:48:33 2026 GMT\n  hsts: false\n- host: studio.palettetechnology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 07:17:59 2026 GMT\n  hsts: false\ndomains:\n- domain: palettetechnology.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palette-2/refs/heads/main/security/palette-2-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Generative AI
- Video Generation
- Media
- Content Generation
- Multimodal
- Creative Tools
---
