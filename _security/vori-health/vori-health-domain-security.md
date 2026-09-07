---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vorihealth.com
  spf: true
hosts:
- cert_expires: Nov 29 22:44:04 2026 GMT
  host: www.vorihealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vori Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vori Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vori Health
provider_slug: vori-health
slug: vori-health-domain-security
source_filename: vori-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vorihealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 22:44:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vorihealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vori-health/refs/heads/main/security/vori-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Care
- Digital Health
- Musculoskeletal
- Telehealth
- Virtual Care
- Physical Therapy
- Orthopedics
- Employer Benefits
- Value-Based Care
- United States
---
