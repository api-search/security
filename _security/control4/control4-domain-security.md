---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: control4.com
  spf: true
hosts:
- cert_expires: Sep 11 21:44:19 2026 GMT
  host: www.control4.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Control4 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Control4, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Control4
provider_slug: control4
slug: control4-domain-security
source_filename: control4-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.control4.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 21:44:19 2026 GMT\n  hsts: false\ndomains:\n- domain: control4.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/control4/refs/heads/main/security/control4-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- IoT
- Smart Home
- Home Automation
- Building Automation
- Lighting Control
- Audio Video
- Drivers
---
