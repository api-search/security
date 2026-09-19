---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aim.vision
  spf: true
hosts:
- cert_expires: Dec 10 20:49:23 2026 GMT
  host: aim.vision
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIM Intelligent Machines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AIM Intelligent Machines
provider_slug: aim
slug: aim-domain-security
source_filename: aim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aim.vision\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 20:49:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aim.vision\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aim/refs/heads/main/security/aim-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Robotics
- Autonomy
- Heavy Equipment
- Earthmoving
- Mining
- Construction
- Defense
- Startups
- General Catalyst Portfolio
---
