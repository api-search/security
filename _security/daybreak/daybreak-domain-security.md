---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daybreakhealth.com
  spf: true
hosts:
- cert_expires: Oct  2 22:01:37 2026 GMT
  host: www.daybreakhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Daybreak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daybreak, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Daybreak
provider_slug: daybreak
slug: daybreak-domain-security
source_filename: daybreak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.daybreakhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 22:01:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: daybreakhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daybreak/refs/heads/main/security/daybreak-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mental Health
- Healthcare
- Teletherapy
- Behavioral Health
- Education
- K-12
- Digital Health
---
