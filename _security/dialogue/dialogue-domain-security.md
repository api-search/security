---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dialogue.co
  spf: true
hosts:
- cert_expires: Sep 20 15:03:30 2026 GMT
  host: www.dialogue.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dialogue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dialogue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dialogue
provider_slug: dialogue
slug: dialogue-domain-security
source_filename: dialogue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dialogue.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:03:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dialogue.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dialogue/refs/heads/main/security/dialogue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Telemedicine
- Virtual Care
- Mental Health
- Employee Assistance Program
- Wellness
- Consumer
- Canada
---
