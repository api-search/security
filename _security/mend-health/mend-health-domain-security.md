---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mend.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: mendfamily.com
  spf: true
hosts:
- cert_expires: Sep 30 06:58:03 2026 GMT
  host: mend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:41:59 2026 GMT
  host: bestservice.mendfamily.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 02:11:08 2026 GMT
  host: api.mendfamily.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mend Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mend, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mend
provider_slug: mend-health
slug: mend-health-domain-security
source_filename: mend-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:58:03 2026 GMT\n  hsts: false\n- host: bestservice.mendfamily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:41:59 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.mendfamily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 02:11:08 2026 GMT\n  hsts: null\ndomains:\n- domain: mend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: mendfamily.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mend-health/refs/heads/main/security/mend-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telehealth
- Telemedicine
- Patient Engagement
- Behavioral Health
- Scheduling
- Video Visits
- Digital Forms
- HIPAA
- Healthcare
---
