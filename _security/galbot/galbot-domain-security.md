---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: galbot.com
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: galbot.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Galbot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for galbot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: galbot
provider_slug: galbot
slug: galbot-domain-security
source_filename: galbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: galbot.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: galbot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galbot/refs/heads/main/security/galbot-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Robotics
- Humanoid Robots
- Embodied AI
- Artificial Intelligence
- Hardware
- China
---
