---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sworkit.com
  spf: true
hosts:
- cert_expires: Sep 26 18:40:22 2026 GMT
  host: sworkit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sworkit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sworkit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sworkit
provider_slug: sworkit
slug: sworkit-domain-security
source_filename: sworkit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sworkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 18:40:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sworkit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sworkit/refs/heads/main/security/sworkit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fitness
- Health & Wellness
- Employee Wellbeing
- Workouts
- Mindfulness
- Nutrition
- Embeddable Components
- SDKs
---
