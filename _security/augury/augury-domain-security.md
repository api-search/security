---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: augury.com
  spf: true
hosts:
- cert_expires: Sep 24 00:22:56 2026 GMT
  host: www.augury.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Augury Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Augury, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Augury
provider_slug: augury
slug: augury-domain-security
source_filename: augury-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.augury.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 00:22:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: augury.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augury/refs/heads/main/security/augury-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Industrial AI
- Machine Health
- Process Health
- Predictive Maintenance
- Vibration Analysis
- Condition Monitoring
- IoT Sensors
- Halo
- Manufacturing
- Reliability
- Asset Performance
- OT
- CMMS
- EAM
---
