---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: beyondimagination.com
  spf: true
hosts:
- cert_expires: Oct 12 00:47:28 2026 GMT
  host: www.beyondimagination.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Beyond Imagination Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beyond Imagination, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Beyond Imagination
provider_slug: beyond-imagination
slug: beyond-imagination-domain-security
source_filename: beyond-imagination-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beyondimagination.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 00:47:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: beyondimagination.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyond-imagination/refs/heads/main/security/beyond-imagination-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Robotics
- Humanoid Robots
- Artificial Intelligence
- Machine-Learning
- Manufacturing
- Automation
- Teleoperation
- Healthcare
- Embodied AI
---
