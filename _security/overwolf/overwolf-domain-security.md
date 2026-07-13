---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: overwolf.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: dev.overwolf.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: www.overwolf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Overwolf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Overwolf, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Overwolf
provider_slug: overwolf
slug: overwolf-domain-security
source_filename: overwolf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.overwolf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: false\n- host: www.overwolf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: overwolf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overwolf/refs/heads/main/security/overwolf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gaming
- In-Game Apps
- Overlays
---
