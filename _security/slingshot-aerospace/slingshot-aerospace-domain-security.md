---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: slingshot.space
  spf: true
hosts:
- cert_expires: Oct  3 03:57:24 2026 GMT
  host: www.slingshot.space
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: portal.slingshot.space
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slingshot Aerospace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slingshot Aerospace, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Slingshot Aerospace
provider_slug: slingshot-aerospace
slug: slingshot-aerospace-domain-security
source_filename: slingshot-aerospace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.slingshot.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:57:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.slingshot.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: slingshot.space\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slingshot-aerospace/refs/heads/main/security/slingshot-aerospace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Space
- Aerospace
- Space Situational Awareness
- Satellite Tracking
- Orbital Intelligence
- Space Domain Awareness
- Defense
- Artificial Intelligence
- Data
---
