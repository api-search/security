---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: augmentus.tech
  spf: true
hosts:
- cert_expires: Aug 22 12:12:32 2026 GMT
  host: augmentus.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Augmentus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Augmentus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Augmentus
provider_slug: augmentus
slug: augmentus-domain-security
source_filename: augmentus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: augmentus.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 12:12:32 2026 GMT\n  hsts: false\ndomains:\n- domain: augmentus.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augmentus/refs/heads/main/security/augmentus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Robotics
- Industrial Automation
- No-Code
- Manufacturing
- Robot Programming
- Computer Vision
- Artificial Intelligence
---
