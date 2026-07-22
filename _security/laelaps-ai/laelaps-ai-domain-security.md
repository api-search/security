---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: laelaps.ai
  spf: true
hosts:
- cert_expires: Oct  5 06:25:05 2026 GMT
  host: laelaps.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Laelaps Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laelaps AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Laelaps AI
provider_slug: laelaps-ai
slug: laelaps-ai-domain-security
source_filename: laelaps-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laelaps.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 06:25:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: laelaps.ai\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laelaps-ai/refs/heads/main/security/laelaps-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Robotics
- Autonomous Systems
- Security
- Surveillance
- Computer Vision
- Defense
- Physical Security
---
