---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: counselhealth.com
  spf: true
hosts:
- cert_expires: Sep  7 04:46:28 2026 GMT
  host: www.counselhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Counsel Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Counsel Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Counsel Health
provider_slug: counsel-health
slug: counsel-health-domain-security
source_filename: counsel-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.counselhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 04:46:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: counselhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/counsel-health/refs/heads/main/security/counsel-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Healthcare
- Telemedicine
- Telehealth
- Primary Care
- Artificial Intelligence
- Embedded API
- Digital Health
---
