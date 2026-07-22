---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: imperfect.co
  spf: true
hosts:
- cert_expires: Sep 27 22:14:04 2026 GMT
  host: imperfect.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imperfect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imperfect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Imperfect
provider_slug: imperfect
slug: imperfect-domain-security
source_filename: imperfect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imperfect.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 22:14:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: imperfect.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imperfect/refs/heads/main/security/imperfect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Fitness
- Wellness
- Sports
- Artificial Intelligence
- Coaching
- Wearables
- Consumer Apps
- Y Combinator
---
