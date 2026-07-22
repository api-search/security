---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caps365.jp
  spf: true
hosts:
- cert_expires: Sep 16 10:33:24 2026 GMT
  host: caps365.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CAPS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CAPS
provider_slug: caps
slug: caps-domain-security
source_filename: caps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caps365.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 10:33:24 2026 GMT\n  hsts: false\ndomains:\n- domain: caps365.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caps/refs/heads/main/security/caps-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Health Management
- Clinics
- Telemedicine
- Corporate Wellness
- Fitness
- Japan
---
