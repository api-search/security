---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: levita.com
  spf: true
hosts:
- cert_expires: Oct  3 04:40:24 2026 GMT
  host: www.levita.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Levita Magnetics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Levita Magnetics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Levita Magnetics
provider_slug: levita-magnetics
slug: levita-magnetics-domain-security
source_filename: levita-magnetics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.levita.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 04:40:24 2026 GMT\n  hsts: false\ndomains:\n- domain: levita.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/levita-magnetics/refs/heads/main/security/levita-magnetics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Surgical Robotics
- Healthcare
- Robotics
- Minimally Invasive Surgery
- Medical Technology
- Hardware
---
