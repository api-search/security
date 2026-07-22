---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intrinsic.ai
  spf: true
hosts:
- cert_expires: Oct  2 04:47:11 2026 GMT
  host: www.intrinsic.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intrinsic Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intrinsic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Intrinsic
provider_slug: intrinsic-ai
slug: intrinsic-ai-domain-security
source_filename: intrinsic-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.intrinsic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 04:47:11 2026 GMT\n  hsts: false\ndomains:\n- domain: intrinsic.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intrinsic-ai/refs/heads/main/security/intrinsic-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Industrial Robotics
- Robotics
- Automation
- Manufacturing
- AI for Robotics
- Embodied AI
- Motion Planning
- Pose Estimation
- Grasp Planning
- Behavior Trees
- Digital Twin
- Simulation
- ROS
- Robot Operating System
- IntrinsicOS
- Flowstate
- Skills
- Services
- Alphabet
- X Moonshot
---
