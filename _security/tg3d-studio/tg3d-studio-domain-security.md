---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tg3ds.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zendesk.com
  spf: true
hosts:
- cert_expires: Sep 27 09:32:27 2026 GMT
  host: tg3ds.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 04:18:02 2026 GMT
  host: tg3ds.zendesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 23:59:59 2027 GMT
  host: api.tg3ds.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tg3D Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TG3D Studio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TG3D Studio
provider_slug: tg3d-studio
slug: tg3d-studio-domain-security
source_filename: tg3d-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tg3ds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:32:27 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: tg3ds.zendesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 04:18:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tg3ds.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: tg3ds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: zendesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tg3d-studio/refs/heads/main/security/tg3d-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- 3D Body Scanning
- Fashion Technology
- Made-to-Measure
- Digital Fashion
- Body Measurement
- Apparel
- API
---
