---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: gymclass.com
  spf: true
hosts:
- cert_expires: Aug 23 00:42:42 2026 GMT
  host: www.gymclass.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gym Class Vr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gym Class VR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Gym Class VR
provider_slug: gym-class-vr
slug: gym-class-vr-domain-security
source_filename: gym-class-vr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gymclass.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 00:42:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gymclass.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gym-class-vr/refs/heads/main/security/gym-class-vr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Virtual Reality
- VR
- Gaming
- Sports
- Meta Quest
- Consumer
- Social
---
