---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lyrahealth.com
  spf: true
hosts:
- cert_expires: Sep  2 23:59:59 2026 GMT
  host: www.lyrahealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lyra Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lyra Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lyra Health
provider_slug: lyra-health
slug: lyra-health-domain-security
source_filename: lyra-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lyrahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lyrahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lyra-health/refs/heads/main/security/lyra-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mental Health
- Behavioral Health
- Employee Benefits
- Enterprise Benefits
- Workforce Wellness
- Employee Assistance Program
- Therapy
- Coaching
- Medication Management
- Pediatric Mental Health
- Family Care
- Telehealth
- Healthcare
- Health Plans
- Artificial Intelligence
- Lyra Empower
- Lyra App
- Centers of Excellence
---
