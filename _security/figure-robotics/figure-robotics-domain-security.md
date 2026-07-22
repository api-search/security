---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: figure.ai
  spf: true
hosts:
- cert_expires: Aug 15 11:25:30 2026 GMT
  host: www.figure.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Figure Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Figure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Figure
provider_slug: figure-robotics
slug: figure-robotics-domain-security
source_filename: figure-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.figure.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 11:25:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: figure.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figure-robotics/refs/heads/main/security/figure-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Humanoid Robots
- General-Purpose Robots
- Embodied AI
- Vision Language Action
- Foundation Models
- Helix
- Figure 03
- Manufacturing
- Home Robotics
- Hardware
---
