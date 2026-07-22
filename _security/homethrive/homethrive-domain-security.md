---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: homethrive.com
  spf: true
hosts:
- cert_expires: Sep  5 18:30:46 2026 GMT
  host: homethrive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Homethrive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Homethrive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Homethrive
provider_slug: homethrive
slug: homethrive-domain-security
source_filename: homethrive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homethrive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 18:30:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: homethrive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homethrive/refs/heads/main/security/homethrive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Caregiving
- Family Caregivers
- Employee Benefits
- Health Plans
- Eldercare
- Backup Care
- Caregiver Support
- Digital Health
- B2B2C
- No Public API
---
