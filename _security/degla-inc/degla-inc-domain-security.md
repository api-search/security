---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: degla.ai
  spf: true
hosts:
- cert_expires: Sep  5 20:28:49 2026 GMT
  host: degla.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Degla Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Degla Inc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Degla Inc
provider_slug: degla-inc
slug: degla-inc-domain-security
source_filename: degla-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: degla.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:28:49 2026 GMT\n  hsts: false\ndomains:\n- domain: degla.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/degla-inc/refs/heads/main/security/degla-inc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Drones
- Autonomous Systems
- Artificial Intelligence
- Aerospace
- Emergency Response
- Robotics
---
